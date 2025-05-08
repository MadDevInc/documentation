# Sistema de Dados
## Visão Geral do Sistema

### Componentes Principais
1. **Dice Slots (dice_slots.gd)**
      - Gerencia a interface de seleção de dados
      - Controla botões de ação (Jogar, Rerolar)
      - Mantém registro dos dados selecionados

2. **Die (die.gd)**
      - Representa um dado físico 3D
      - Calcula o valor resultante da rolagem
      - Gerencia efeitos visuais e físicos

## Tabela de Funcionalidades

| Componente                  | Funcionalidade    | Descrição                            | Parâmetros                | Efeitos                                  |
| --------------------------- | ----------------- | ------------------------------------ | ------------------------- | ---------------------------------------- |
| `add_dice`                  | Adição de dados   | Adiciona novo dado à área de seleção | `value`: Valor do dado    | Atualiza contagem, verifica limites      |
| `select_die`                | Seleção de dado   | Marca dado para ações futuras        | `die`: Referência ao dado | Ativa botões quando 5 dados selecionados |
| `deselect_die`              | Desseleção        | Remove dado da seleção atual         | `die`: Referência ao dado | Desativa botões se seleção vazia         |
| `_on_play_button_pressed`   | Ação de jogar     | Confirma seleção de dados            | -                         | Envia dados para lógica principal        |
| `_on_reroll_button_pressed` | Rerolagem         | Substitui dados selecionados         | -                         | Remove e solicita novos dados            |
| `_process` (Die)            | Detecção de valor | Calcula face superior após rolagem   | -                         | Determina valor final do dado            |
| `kill`                      | Efeito visual     | Remove dado com partículas           | -                         | Efeito de destruição ao desaparecer      |

## Fluxo de Jogo

1. **Rolagem Inicial**:
      - Dados físicos são rolados na cena 3D
      - Sistema detecta quando dados param de se mover
      - Valores são calculados baseados na face superior

2. **Seleção de Dados**:
      - Jogador seleciona até 5 dados
      - Botões são ativados/desativados conforme seleção
      - Efeitos sonoros acompanham interações

3. **Ações Disponíveis**:
      - **Jogar**: Confirma seleção atual
      - **Rerolar**: Substitui dados selecionados (limitado)

## Especificações Técnicas

### Dice Slots
- Capacidade máxima: 7 dados visíveis
- Requisito para jogar: 5 dados selecionados
- Controles:
    - `play_button`: Só ativo com 5 dados
    - `reroll_button`: Ativo com seleção e rerolls disponíveis

### Die (Dado 3D)
- Física realista com rotação aleatória inicial
- Sistema de detecção:
    - Usa Raycasts para determinar face superior
    - Valor calculado como `7 - face_inferior`
- Efeitos:
    - Partículas de destruição ao remover
    - Sons de interação

## Balanceamento e Regras

1. **Limites**:
      - Máximo 7 dados na área de seleção
      - Necessário selecionar exatamente 5 para jogar

2. **Rerolls**:
      - Quantidade controlada pelo sistema pai
      - Só disponível para dados selecionados

3. **Física**:
      - Dados recebem rotação aleatória inicial
      - Devem estar completamente parados para registro do valor

## Próximos Passos

1. **Novos Tipos de Dados**:
      - Dados com mais números de lados
      - Dados bônus com efeitos únicos

2. **Modificadores Visuais**:
      - Destaque para dados selecionados
      - Animação ao confirmar seleção

3. **Sistema de Combinação**:
      - Bônus por combinar certos tipos de dados (cores de dados)
      - Efeitos especiais para combinações raras