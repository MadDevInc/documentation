# Módulo de Game Design: Núcleo do Jogo

Este documento detalha o sistema central do jogo, incluindo fluxo principal, mecânicas de combate e progressão.

## Visão Geral do Sistema

### Componentes Principais
1. **Game Manager** (`Game.gd`)   - Controla o fluxo principal do jogo
2. **Sistema de Cartas** (`switch_card.gd`, `ui_card.gd`)   - Gerencia seleção de cartas
3. **Sistema de Derrota** (`loss.gd`)   - Trata estado de game over
4. **Player Manager** (`player.gd`)   - Gerencia dados do jogador

## Fluxo Principal do Jogo

```mermaid
graph TD
    A[Seleção de Cartas]   -  -> B[Transição]
    B   -  -> C[Fase de Combate]
    C   -  -> D{Vitória?}
    D   -  ->|Sim| E[Próxima Fase]
    D   -  ->|Não| F[Tela de Derrota]
    E   -  -> B
    F   -  -> G[Menu Principal/Repetir]
```

## Mecânicas de Combate

### Sequência de Turno
1. **Rolagem de Dados**:
     - Jogador rola 7 dados 3D
     - Seleciona 5 para usar no combate

2. **Aplicação de Modificadores**:
     - Cartas do jogador são aplicadas
     - Modificadores do inimigo são aplicados

3. **Resolução**:
     - Comparação de valores modificados
     - Determinação do vencedor do round

4. **Progressão**:
     - Melhor de 3 rounds
     - 4 fases no total

### Sistemas Integrados

| Sistema    | Arquivo          | Responsabilidade                      |
|   -  -  -  -  -  -  -  -  -  - |   -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  - |   -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  - |
| Dados      | `Game.gd`        | Rolagem, seleção e cálculo de valores |
| Cartas     | `switch_card.gd` | Seleção de habilidades passivas       |
| Inimigos   | `Game.gd`        | Comportamento e modificadores         |
| Progressão | `transition.gd`  | Controle de fases e dificuldade       |

## Tabela de Estados do Jogo

| Estado            | Condição de Entrada | Ações                        | Transições Possíveis   |
|   -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  - |   -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  - |   -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  - |   -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  - |
| Seleção de Cartas | Início de fase      | Oferece 2 cartas aleatórias  | Transição para combate |
| Combate           | Após transição      | Rolagem e resolução de dados | Vitória/Derrota        |
| Vitória           | Ganhar 2 rounds     | Animação, incremento de fase | Transição ou Final     |
| Derrota           | Perder 2 rounds     | Mostra estatísticas          | Menu/Repetir           |

## Balanceamento e Progressão

1. **Dificuldade Progressiva**:
     - Inimigos ganham modificadores mais fortes
     - Número de rerolls pode diminuir

2. **Sistema de Cartas**:
     - Cartas oferecem combos estratégicos
     - Novas cartas desbloqueadas progressivamente

3. **Pontuação**:
     - Maior rolagem registrada
     - Inimigos derrotados como métrica

## Detalhes de Implementação

### Combate (Game.gd)
```gdscript
func play_dice(selection: Array):
    # 1. Movimentação visual
    await move_dice_to_center(selection)
    
    # 2. Cálculo de valores
    await count_dice_player(selection)
    
    # 3. Aplicação de modificadores
    await apply_player_modifiers()
    
    # 4. Resolução do inimigo
    await enemy_sum_count()
    var result = await apply_enemy_modifiers()
    
    # 5. Determinação do vencedor
    await decide_winner(result)
```

### Seleção de Cartas
```gdscript
func handle_card_selection(selected_card):
    Global.deck_player.append(selected_card)
    disable_cards()
    play_outro_animation()
```

### Derrota
```gdscript
func _on_retry_button_pressed():
    Global.reset_stats()
    $AnimationPlayer.play("outro")
    retry = true
```

## Próximos passos

1. **Adicionar os elementos de rogue-like**:
     - Caminhos alternativos após um encontro
     - Encontros aleatórios
     - Sistema de mapa com trilhas

2. **Profundidade Estratégica**:
     - Combos entre cartas específicas
     - Dados com habilidades especiais

3. **Progressão Meta**:
     - Desbloqueio de cartas permanentes
     - Melhorias para modificadores