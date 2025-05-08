# Sistema de Cartas
## Cartas do Jogador

### Visão Geral do Sistema

As cartas são implementadas como:
- Componentes visuais controlados por `card.gd`
- Modificadores de jogabilidade em `cards_modifiers.gd`
- Efeitos são aplicados automaticamente após rolagem de dados
- Cada carta tem um tipo associado que determina seu efeito

### Tabela de Cartas Implementadas

| Nome da Carta | Tipo         | Efeito                          | Condição de Ativação                   | Fórmula de Pontuação                    | Observações                             |
| ------------- | ------------ | ------------------------------- | -------------------------------------- | --------------------------------------- | --------------------------------------- |
| Full House    | FULL_HOUSE   | Bônus por combinação específica | Dois dados de um valor e três de outro | Soma dos dois valores distintos         | Ex: [2,2,5,5,5] → 2+5=7 pontos extras   |
| Sequência     | SEQUENCIA    | Bônus por números consecutivos  | 3+ números em sequência                | 1.5 pontos por número na sequência      | Sequência máxima encontrada             |
| Cinco Iguais  | CINCO_IGUAIS | Bônus por dados idênticos       | Todos os 5 dados com mesmo valor       | Valor do dado (ex: cinco 4s = 4 pontos) | Aplica apenas o valor do dado           |
| Modificador   | MODIFICADOR  | (Não implementado)              | -                                      | -                                       | Placeholder para futuras implementações |

### Detalhes de Implementação

***Fluxo do Sistema***

1. O jogador rola os dados
2. `cards_modifiers.gd` itera por todas as cartas do jogador
3. Para cada carta, verifica o tipo e aplica a função correspondente
4. Modificadores são aplicados na variável `player_sum_modified`

***Código dos Efeitos***
```gdscript
# Exemplo: Full House
if counts == [2, 3]:
    var modified_score : int = (values[0] + values[1])
    PlayerManager.player_sum_modified += modified_score
```

### Balanceamento Atual

- **Full House**: Valor relativamente baixo (soma dos pares)
- **Sequência**: Progressivo (1.5pt por número)
- **Cinco Iguais**: Valor fixo do dado

### Próximos Passos:

1. Adicionar cartas com efeitos:
      - Multiplicadores
      - Bônus por combinações específicas
      - Efeitos condicionais
2. Implementar sistema de níveis para cartas
3. Adicionar descrições detalhadas nas tooltips
---
## Cartas do Inimigo
Este documento detalha os modificadores que os inimigos podem aplicar durante o jogo, conforme implementado em `enemy_modifiers.gd`.

### Visão Geral do Sistema

- Modificadores são habilidades passivas dos inimigos
- Afetam diretamente o resultado da partida
- Podem alterar quem é declarado vencedor
- Alguns aplicam penalidades diretas ao jogador

### Tabela de Modificadores Implementados

| Nome do Modificador | Tipo          | Efeito                         | Condição de Ativação              | Impacto no Jogo                        |
| ------------------- | ------------- | ------------------------------ | --------------------------------- | -------------------------------------- |
| Número Ímpar        | NUMERO_IMPAR  | Declara inimigo vencedor       | Soma do jogador é ímpar           | Inimigo vence automaticamente          |
| Número Par          | NUMERO_PAR    | Declara inimigo vencedor       | Soma do jogador é par             | Inimigo vence automaticamente          |
| Número Menor        | NUMERO_MENOR  | Comparação de valores          | Soma do jogador < Soma do inimigo | Inimigo vence se condição for atendida |
| Número Maior        | NUMERO_MAIOR  | Comparação de valores          | Soma do jogador > Soma do inimigo | Jogador vence se condição for atendida |
| Número Vetado       | NUMERO_VETADO | Penalidade por dado específico | Jogador tirou o número 6          | Reduz 6 pontos da soma do jogador      |

### Detalhes de Implementação

#### Fluxo do Sistema
1. Após a rolagem de dados:
   - Verifica cada modificador do inimigo
   - Aplica os efeitos condicionais
   - Pode alterar o vencedor ou modificar pontuações

#### Código de Exemplo
```gdscript
func numero_vetado():
    if PlayerManager.current_player_dice.has(6):
        EnemyManager.punicao = 6
        PlayerManager.player_sum_modified -= EnemyManager.punicao
```

### Balanceamento e Regras

1. ***Modificadores Absolutos*** (Ímpar/Par):
      - Ignoram a comparação normal de pontos
      - Criam situações de vitória automática

2. ***Modificadores Comparativos*** (Maior/Menor):
      - Mantêm a dinâmica normal do jogo
      - Apenas invertem a condição de vitória

3. ***Modificador de Penalidade*** (Vetado):
      - Punitivo quando aparece o número 6
      - Redução fixa de 6 pontos

### Próximos Passos:

1. Adicionar novos modificadores:
      - "Dobro": Dobra a pontuação do inimigo se condição for atendida
      - "Sorte": Rola um dado extra para o inimigo
      - "Azar": Remove o maior dado do jogador
2. Adicionar efeitos visuais:
      - Feedback claro quando modificador é ativado
      - Ícones diferentes para cada tipo