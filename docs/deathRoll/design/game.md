# Backlog - Death Roll

## Temas (TM)

Os temas representam as áreas principais do desenvolvimento do jogo.

| ID   | Nome                  | Descrição                                                      |
| ---- | --------------------- | -------------------------------------------------------------- |
| TM01 | Arte e Design         | Criação de cenários, personagens, itens e conceitos visuais.   |
| TM02 | Jogabilidade          | Desenvolvimento de mecânicas de combate, mini-games e eventos. |
| TM03 | Interface do Usuário  | Criação de menus e interações acessíveis e intuitivas.         |
| TM04 | Áudio e Trilha Sonora | Composição de músicas e efeitos sonoros imersivos.             |
| TM05 | Narrativa e Mundo     | Construção da história, ambientação e progressão do jogador.   |

---

## Épicos (EP)

Os épicos são grandes blocos de trabalho dentro de cada tema.

### TM01 - Arte e Design

| ID   | Nome                     | Descrição                                               |
| ---- | ------------------------ | ------------------------------------------------------- |
| EP01 | Criação de Cenários      | Desenvolvimento de 9 cenários distintos para o jogo.    |
| EP02 | Modelagem de Personagens | Modelagem de inimigos, NPCs e outros elementos visuais. |
| EP03 | Design de Itens          | Criação de dados, cartas, baús e outros objetos.        |

### TM02 - Jogabilidade

| ID   | Nome                  | Descrição                                                           |
| ---- | --------------------- | ------------------------------------------------------------------- |
| EP04 | Combate               | Desenvolvimento de mecânicas de combate baseadas em dados e cartas. |
| EP05 | Mini-Games            | Implementação de mini-games para eventos aleatórios.                |
| EP06 | Sistema de Progressão | Criação de mecânicas de progressão e escolha de caminhos.           |

### TM03 - Interface do Usuário

| ID   | Nome                  | Descrição                                                                |
| ---- | --------------------- | ------------------------------------------------------------------------ |
| EP07 | Menus de Navegação    | Criação de menus para loja, deck, dados, pausa e diálogo.                |
| EP08 | HUD e Feedback Visual | Desenvolvimento de elementos visuais para exibir informações ao jogador. |

### TM04 - Áudio e Trilha Sonora

| ID   | Nome                  | Descrição                                                          |
| ---- | --------------------- | ------------------------------------------------------------------ |
| EP09 | Composição de Músicas | Criação de trilhas sonoras temáticas para cada círculo do Inferno. |
| EP10 | Efeitos Sonoros       | Desenvolvimento de sons para ações e ambientação.                  |

### TM05 - Narrativa e Mundo

| ID   | Nome                           | Descrição                                                    |
| ---- | ------------------------------ | ------------------------------------------------------------ |
| EP11 | Construção do Mundo            | Desenvolvimento dos 9 círculos do Inferno, Purgatório e Céu. |
| EP12 | Desenvolvimento de Personagens | Criação de personagens como Virgílio, Beatriz e chefes.      |

---

## Capacidades (C)

As capacidades detalham os objetivos específicos de cada épico.

### EP01 - Criação de Cenários

| ID  | Nome               | Descrição                                                     |
| --- | ------------------ | ------------------------------------------------------------- |
| C01 | Design de Cenários | Criar 9 cenários distintos com estética única.                |
| C02 | Ambientação Visual | Adicionar elementos visuais que reforcem a narrativa do jogo. |

### EP04 - Combate

| ID  | Nome                | Descrição                                                   |
| --- | ------------------- | ----------------------------------------------------------- |
| C03 | Sistema de Dados    | Implementar mecânicas de lançamento e manipulação de dados. |
| C04 | Sistema de Cartas   | Desenvolver mecânicas para uso de cartas no combate.        |
| C05 | Feedback de Combate | Exibir informações como vida, combos e jogadas do inimigo.  |

### EP07 - Menus de Navegação

| ID  | Nome           | Descrição                                              |
| --- | -------------- | ------------------------------------------------------ |
| C06 | Menu Principal | Criar menu inicial com opções de jogo e configurações. |
| C07 | Menu da Loja   | Desenvolver interface para compra e venda de itens.    |
| C08 | Menu do Deck   | Criar interface para visualização e edição do baralho. |

---

## Funcionalidades (F)

As funcionalidades são tarefas específicas que implementam as capacidades.

### C03 - Sistema de Dados

| ID  | Nome              | Descrição                                             |
| --- | ----------------- | ----------------------------------------------------- |
| F01 | Lançar Dados      | Permitir que o jogador lance dados durante o combate. |
| F02 | Rolar Novamente   | Implementar a opção de reroll para dados específicos. |
| F03 | Exibir Resultados | Mostrar os valores finais dos dados lançados.         |

### C07 - Menu da Loja

| ID  | Nome          | Descrição                                                |
| --- | ------------- | -------------------------------------------------------- |
| F04 | Comprar Itens | Permitir que o jogador compre cartas e dados.            |
| F05 | Vender Itens  | Permitir que o jogador venda cartas para obter recursos. |

---

## Histórias de Usuário (US)

As histórias de usuário detalham as interações do jogador com o sistema.

| ID   | Nome                      | Funcionalidade | Descrição                                                                             |
| ---- | ------------------------- | -------------- | ------------------------------------------------------------------------------------- |
| US01 | Criar Cenários            | F01            | Como designer, quero criar 9 cenários distintos para enriquecer o jogo.               |
| US02 | Jogar Dados no Combate    | F01            | Como jogador, quero lançar dados para atacar inimigos durante o combate.              |
| US03 | Participar de Mini-Games  | F03            | Como jogador, quero participar de mini-games para ganhar recompensas.                 |
| US04 | Navegar pelos Menus       | F04            | Como jogador, quero acessar menus intuitivos para gerenciar meu progresso.            |
| US05 | Explorar o Mapa           | F05            | Como jogador, quero explorar o mapa e encontrar encontros aleatórios.                 |
| US06 | Comprar Cartas na Loja    | F04            | Como jogador, quero comprar cartas na loja para melhorar meu baralho.                 |
| US07 | Usar Artefatos no Combate | F03            | Como jogador, quero usar artefatos durante o combate para alterar o curso da batalha. |

---

## Histórico de Revisões

| Data       | Autor                                      | Alterações                                         |
| ---------- | ------------------------------------------ | -------------------------------------------------- |
| 2025-05-13 | [Mateus Vieira](https://github.com/matix0) | Reestruturação do backlog para maior consistência. |
