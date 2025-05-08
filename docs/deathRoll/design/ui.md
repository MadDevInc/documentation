# Elementos de UI

## Visão Geral do Sistema

### Componentes Principais
1. **Sistema de Transição** (`transition.gd`)
2. **Contador de Pontuação** (`score_counter.gd`)
3. **Gerenciador de Rerolls** (`reroll_count.gd` e `reroll_icon.gd`)
4. **Efeitos Visuais** (`die_kill.gd`)
5. **Botões Interativos** (`Button.gd`)

## Tabela de Componentes de UI

| Componente               | Arquivo            | Função Principal                      | Propriedades                    | Comportamento                         |
| ------------------------ | ------------------ | ------------------------------------- | ------------------------------- | ------------------------------------- |
| Transição entre Cenas    | `transition.gd`    | Gerencia mudanças de fase             | - `Global.stage`                | Reproduz animação específica por fase |
| Contador de Pontos       | `score_counter.gd` | Controla progresso do jogador         | - `max_points` (exportado)      | Emite sinal de vitória ao completar   |
| Ícone de Reroll          | `reroll_icon.gd`   | Representa uma reroll disponível      | -                               | Animação ao ser consumido             |
| Gerenciador de Rerolls   | `reroll_count.gd`  | Controla rerolls disponíveis          | - `max_rerolls`                 | Adiciona/remove ícones visualmente    |
| Efeito de Dado Destruído | `die_kill.gd`      | Feedback visual para remoção de dados | - `initial_position`            | Partículas e efeito sonoro            |
| Botão Genérico           | `Button.gd`        | Base para interações                  | - `normal`/`pressed` (texturas) | Muda estado visual ao interagir       |

## Detalhes de Implementação

### Sistema de Transição
```gdscript
func _ready():
    Global.stage += 1
    var animation = "goto" + str(Global.stage)
    anims.play(animation)
```
- Incrementa fase global automaticamente
- Carrega animação específica para cada fase (ex: "goto1", "goto2")
- Mudança de cena ocorre ao final da animação "outro"

### Contador de Pontos
1. Inicializa com ícones vazios
2. `add_point()` preenche ícones sequencialmente
3. Ao atingir `max_points`, emite sinal de vitória

### Sistema de Rerolls
| Ação                      | Método           | Efeito                          |
| ------------------------- | ---------------- | ------------------------------- |
| Consumir reroll           | `spend_reroll()` | Executa animação e remove ícone |
| Verificar disponibilidade | `rerolls_left()` | Retorna quantidade restante     |
| Adicionar reroll          | `add_reroll()`   | Instancia novo ícone            |

### Botão Interativo
**Estados:**

- `active=true`: Totalmente visível, interativo
- `active=false`: Semitransparente, não interativo

**Comportamento:**

- Muda textura quando pressionado
- Emite sinal `button_pressed` apenas quando ativo

## Fluxo de Interação

1. **Progressão de Fase**:
    - Animação de transição inicia automaticamente
    - Ao final, carrega nova cena de jogo

2. **Pontuação**:
    - Cada ponto adicionado dispara animação "pop"
    - Vitória é automaticamente detectada

3. **Rerolls**:
    - Ícones são consumidos da direita para esquerda
    - Cada consumo toca animação antes de desaparecer

4. **Feedback Visual**:
    - Dados destruídos emitem partículas vermelhas/pretas
    - Efeito sonoro acompanha a destruição

## Próximos Passos:

1. **Melhorias Visuais**:
    - Animação de preenchimento progressivo para pontos
    - Efeito de pulsação para rerolls disponíveis
    - Transições personalizadas por tipo de fase

2. **Novos Componentes**:
    - Notificações flutuantes para eventos importantes
    - Menu contextual com informações de jogo