# Cartas do Inimigo

## Visão Geral do Sistema

As cartas do inimigo são implementadas como:
- Modificadores passivos controlados por `enemy_modifiers.gd`.
- Afetam diretamente o resultado da partida.
- Podem alterar quem é declarado vencedor ou aplicar penalidades ao jogador.

## Tabela de Modificadores Implementados

| Nome do Modificador | Tipo          | Efeito                         | Condição de Ativação              | Impacto no Jogo                        |
| ------------------- | ------------- | ------------------------------ | --------------------------------- | -------------------------------------- |
| Número Ímpar        | NUMERO_IMPAR  | Declara inimigo vencedor       | Soma do jogador é ímpar           | Inimigo vence automaticamente          |
| Número Par          | NUMERO_PAR    | Declara inimigo vencedor       | Soma do jogador é par             | Inimigo vence automaticamente          |
| Número Menor        | NUMERO_MENOR  | Comparação de valores          | Soma do jogador < Soma do inimigo | Inimigo vence se condição for atendida |
| Número Maior        | NUMERO_MAIOR  | Comparação de valores          | Soma do jogador > Soma do inimigo | Jogador vence se condição for atendida |
| Número Vetado       | NUMERO_VETADO | Penalidade por dado específico | Jogador tirou o número 6          | Reduz 6 pontos da soma do jogador      |

## Detalhes de Implementação

1. Após a rolagem de dados:
   - Verifica cada modificador do inimigo.
   - Aplica os efeitos condicionais.
   - Pode alterar o vencedor ou modificar pontuações.

## Próximos Passos

1. Adicionar novos modificadores:
   - "Dobro": Dobra a pontuação do inimigo se condição for atendida.
   - "Sorte": Rola um dado extra para o inimigo.
   - "Azar": Remove o maior dado do jogador.
2. Adicionar efeitos visuais:
   - Feedback claro quando modificador é ativado.
   - Ícones diferentes para cada tipo.