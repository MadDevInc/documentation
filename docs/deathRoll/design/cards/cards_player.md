# Cartas do Jogador

## Visão Geral do Sistema

As cartas do jogador são implementadas como:
- Componentes visuais controlados por `card.gd`.
- Modificadores de jogabilidade em `cards_modifiers.gd`.
- Efeitos aplicados automaticamente após a rolagem de dados.

## Tabela de Cartas Implementadas

| Nome da Carta | Tipo         | Efeito                          | Condição de Ativação                   | Fórmula de Pontuação                    | Observações                             |
| ------------- | ------------ | ------------------------------- | -------------------------------------- | --------------------------------------- | --------------------------------------- |
| Full House    | FULL_HOUSE   | Bônus por combinação específica | Dois dados de um valor e três de outro | Soma dos dois valores distintos         | Ex: [2,2,5,5,5] → 2+5=7 pontos extras   |
| Sequência     | SEQUENCIA    | Bônus por números consecutivos  | 3+ números em sequência                | 1.5 pontos por número na sequência      | Sequência máxima encontrada             |
| Cinco Iguais  | CINCO_IGUAIS | Bônus por dados idênticos       | Todos os 5 dados com mesmo valor       | Valor do dado (ex: cinco 4s = 4 pontos) | Aplica apenas o valor do dado           |

## Detalhes de Implementação

1. O jogador rola os dados.
2. `cards_modifiers.gd` itera por todas as cartas do jogador.
3. Para cada carta, verifica o tipo e aplica a função correspondente.
4. Modificadores são aplicados na variável `player_sum_modified`.

## Próximos Passos

1. Adicionar cartas com efeitos:
   - Multiplicadores.
   - Bônus por combinações específicas.
   - Efeitos condicionais.
2. Implementar sistema de níveis para cartas.
3. Adicionar descrições detalhadas nas tooltips.