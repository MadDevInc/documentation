# Deck Completo

Este documento contém todas as cartas desenvolvidas até o momento, separadas entre cartas do jogador e modificadores do inimigo.

## Cartas do Jogador

| Nome da Carta  | Tipo         | Efeito                          | Condição de Ativação                   | Impacto no Jogo                        |
| -------------- | ------------ | ------------------------------- | -------------------------------------- | -------------------------------------- |
| Full House     | FULL_HOUSE   | Bônus por combinação específica | Dois dados de um valor e três de outro | Soma dos dois valores distintos         |
| Sequência      | SEQUENCIA    | Bônus por números consecutivos  | 3+ números em sequência                | 1.5 pontos por número na sequência      |
| Cinco Iguais   | CINCO_IGUAIS | Bônus por dados idênticos       | Todos os 5 dados com mesmo valor       | Valor do dado (ex: cinco 4s = 4 pontos) |

## Cartas do Inimigo

| Nome do Modificador | Tipo          | Efeito                         | Condição de Ativação              | Impacto no Jogo                        |
| ------------------- | ------------- | ------------------------------ | --------------------------------- | -------------------------------------- |
| Número Ímpar        | NUMERO_IMPAR  | Declara inimigo vencedor       | Soma do jogador é ímpar           | Inimigo vence automaticamente           |
| Número Par          | NUMERO_PAR    | Declara inimigo vencedor       | Soma do jogador é par             | Inimigo vence automaticamente           |
| Número Menor        | NUMERO_MENOR  | Comparação de valores          | Soma do jogador < Soma do inimigo | Inimigo vence se condição for atendida  |
| Número Maior        | NUMERO_MAIOR  | Comparação de valores          | Soma do jogador > Soma do inimigo | Jogador vence se condição for atendida  |
| Número Vetado       | NUMERO_VETADO | Penalidade por dado específico | Jogador tirou o número 6          | Reduz 6 pontos da soma do jogador       |

## Próximos Passos

1. Adicionar novas cartas e modificadores:
   - **Jogador**:
     - Multiplicadores.
     - Bônus por combinações específicas.
     - Efeitos condicionais.
   - **Inimigo**:
     - "Dobro": Dobra a pontuação do inimigo se condição for atendida.
     - "Sorte": Rola um dado extra para o inimigo.
     - "Azar": Remove o maior dado do jogador.
2. Balancear os efeitos existentes.
3. Implementar efeitos visuais e descrições detalhadas.