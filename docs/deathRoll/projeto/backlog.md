# Backlog - Death Roll

O Backlog de Requisitos do projeto é concebido como um documento vivo, passível de atualização conforme a evolução do desenvolvimento. Seu principal objetivo é orientar toda a equipe na direção da meta estabelecida, assegurando a entrega de valor máximo ao jogo.

## Estrutura do Backlog

Os requisitos estão organizados em uma hierarquia estruturada da seguinte forma:

| Categoria                                                 | Descrição                                                                                                                                                                     | Como Usar                                                                                                              |
| --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| [**Temas (TM)**](#temas-tm)                               | Representam as áreas principais do desenvolvimento do jogo, como Arte e Design, Jogabilidade, Interface do Usuário, Áudio e Trilha Sonora e Narrativa e Mundo.                | Escolha um tema para identificar a área de trabalho que será abordada (ex.: "Jogabilidade" para mecânicas de combate). |
| [**Épicos (EP)**](#epicos-ep)                             | São grandes blocos de trabalho dentro de cada tema. Eles descrevem objetivos amplos, como "Criação de Cenários" ou "Desenvolvimento de Mini-Games".                           | Divida o trabalho em épicos para organizar tarefas maiores dentro de cada tema.                                        |
| [**Capacidades (C)**](#capacidades-c)                     | Detalham os objetivos específicos de cada épico. Por exemplo, no épico "Combate", uma capacidade seria "Implementar mecânicas de lançamento de dados".                        | Use as capacidades para descrever o que precisa ser feito para alcançar o objetivo do épico.                           |
| [**Funcionalidades (F)**](#funcionalidades-f)             | São tarefas específicas que implementam as capacidades. Por exemplo, "Permitir que o jogador lance dados durante o combate".                                                  | Planeje e execute funcionalidades como tarefas individuais ou em sprints.                                              |
| [**Histórias de Usuário (US)**](#historias-de-usuario-us) | Detalham as interações do jogador com o sistema, sempre do ponto de vista do usuário. Por exemplo, "Como jogador, quero lançar dados para atacar inimigos durante o combate". | Use histórias de usuário para entender as necessidades do jogador e priorizar funcionalidades que entreguem valor.     |
| [**Arte Conceito (AC)**](#arte-conceito-ac)               | Detalha os contextos visuais do jogo, como ambiente, cenários, criaturas, interfaces, etc.                                                                                   | Utilize para definir o estilo e direção artística, servindo como referência para a equipe de arte.                     |
| [**Requisitos de Áudio (RA)**](#requisitos-de-audio-ra)   | Especifica as necessidades técnicas e criativas da sonorização do jogo, incluindo trilha, efeitos e integração com a gameplay.                                               | Documente os requisitos para garantir que o áudio esteja alinhado com a experiência desejada do jogo.                  |
| [**Histórico de Revisões**](#histórico-de-revisões)                             | Registra as alterações feitas no backlog, incluindo a data, o autor e uma breve descrição das mudanças.                                                                       | Consulte o histórico para acompanhar a evolução do backlog e manter a rastreabilidade.                                 |

## Temas (TM)

Os temas representam as áreas centrais do desenvolvimento do jogo.

| ID   | Nome                  | Descrição                                                             |
| ---- | --------------------- | --------------------------------------------------------------------- |
| TM01 | Arte e Design         | Criação de cenários, personagens, itens e conceitos visuais.          |
| TM02 | Jogabilidade          | Desenvolvimento de mecânicas de combate, Eventos Aleatóriose eventos. |
| TM03 | Interface do Usuário  | Criação de menus e interações acessíveis e intuitivas.                |
| TM04 | Áudio e Trilha Sonora | Composição de músicas e efeitos sonoros imersivos.                    |
| TM05 | Narrativa e Mundo     | Construção da história, ambientação e progressão do jogador.          |

---

## Épicos (EP)

São grandes blocos de trabalho dentro de cada tema.

| Tema                  | ID   | Nome                   | Descrição                                                                                    |
| --------------------- | ---- | ---------------------- | -------------------------------------------------------------------------------------------- |
| Arte e Design         | EP01 | Criação de Cenários    | Desenvolvimento de 9 cenários distintos para o jogo.                                         |
| Arte e Design         | EP02 | Criação de Personagens | Modelagem de inimigos, NPCs e outros elementos visuais.                                      |
| Arte e Design         | EP03 | Design de Itens        | Criação de dados, cartas, baús e outros objetos.                                             |
| Jogabilidade          | EP04 | Combate                | Desenvolvimento de mecânicas de combate baseadas em dados e cartas.                          |
| Jogabilidade          | EP05 | Eventos Aleatórios     | Implementação de Eventos Aleatórios                                                          |
| Jogabilidade          | EP06 | Sistema de Trilha      | Criação de mecânicas de progressão de níveis com escolha de caminhos aleatóriamente gerados. |
| Jogabilidade          | EP07 | Loja                   | Criação de uma loja para compra de cartas                                                    |
| Interface do Usuário  | EP08 | Menus de Navegação     | Criação de menus para loja, deck, dados, pausa e diálogo.                                    |
| Interface do Usuário  | EP09 | HUD e Feedback Visual  | Desenvolvimento de elementos visuais para exibir informações ao jogador.                     |
| Áudio e Trilha Sonora | EP10 | Composição de Músicas  | Criação de trilhas sonoras temáticas para cada círculo do Inferno.                           |
| Áudio e Trilha Sonora | EP11 | Efeitos Sonoros        | Desenvolvimento de sons para ações e ambientação.                                            |
| Narrativa e Mundo     | EP12 | Diálogos               | Criação dos diálogos do jogo.                                                                |

---

## Capacidades (C)

Capacidades descrevem objetivos específicos vinculados a cada épico.

| Épico                         | ID  | Capacidade                                                          |
| ----------------------------- | --- | ------------------------------------------------------------------- |
| EP01 - Criação de Cenários    | C01 | Criar cenários únicos para cada círculo do Inferno                  |
| EP01 - Criação de Cenários    | C02 | Otimizar performance visual dos cenários                            |
| EP02 - Criação de Personagens | C03 | Criar modelos 2D para NPCs e inimigos                               |
| EP02 - Criação de Personagens | C04 | Integrar personagens com sistema de combate                         |
| EP03 - Design de Itens        | C05 | Criar visuais distintos para cada item                              |
| EP03 - Design de Itens        | C06 | Integrar itens com sistema de menu (saco de dados e deck)           |
| EP04 - Combate                | C07 | Implementar sistema de lançamento de dados                          |
| EP04 - Combate                | C08 | Implementar o sistema das cartas                                    |
| EP05 - Eventos Aleatórios     | C09 | Gerar eventos com consequências variadas                            |
| EP05 - Eventos Aleatórios     | C10 | Integrar eventos aleatórios ao fluxo de gameplay                    |
| EP06 - Sistema de Trilha      | C11 | Gerar caminhos de progressão aleatórios entre níveis                |
| EP06 - Sistema de Trilha      | C12 | Exibir mapa da trilha com opções de escolha visíveis ao jogador     |
| EP07 - Loja                   | C13 | Implementar interface de compra de cartas                           |
| EP07 - Loja                   | C14 | Programar sistema de moedas e economia                              |
| EP08 - Menus de Navegação     | C15 | Criar estrutura de menus                                            |
| EP08 - Menus de Navegação     | C16 | Implementar transições visuais entre menus                          |
| EP09 - HUD e Feedback Visual  | C17 | Mostrar informações de combate e status do jogador                  |
| EP09 - HUD e Feedback Visual  | C18 | Exibir efeitos visuais em ações como dano ou combo                  |
| EP10 - Composição de Músicas  | C19 | Criar trilhas sonoras adaptadas a cada círculo do Inferno           |
| EP10 - Composição de Músicas  | C20 | Implementar variações dinâmicas na música conforme ações do jogador |
| EP11 - Efeitos Sonoros        | C21 | Adicionar sons para interações, menus e ações de combate            |
| EP11 - Efeitos Sonoros        | C22 | Integrar efeitos sonoros com sistema de animação                    |
| EP14 - Diálogos               | C27 | Escrever os diálogos do jogo                                        |
| EP14 - Diálogos               | C28 | Implementar sistema de taunt de elites e boss para o jogador        |
| EP03 - Design de Itens        | C29 | Integrar o sistema de artefatos                                     |

## Funcionalidades (F)

As funcionalidades são tarefas técnicas concretas que implementam as capacidades.

| Capacidade ()                                                             | ID  | Funcionalidade                                                            |
| ------------------------------------------------------------------------- | --- | ------------------------------------------------------------------------- |
| C01 - Criar cenários únicos para cada círculo do Inferno                  | F01 | Criar um fundo temático para cada círculo                                 |
| C03 - Criar modelos 2D para NPCs e inimigos                               | F02 | Criar os sprites para os inimigos                                         |
| C03 - Criar modelos 2D para NPCs e inimigos                               | F03 | Criar os sprites NPCs                                                     |
| C04 - Integrar personagens com sistema de combate                         | F04 | Integrar eventos de animação com sistema de combate                       |
| C05 - Criar visuais distintos para cada item                              | F05 | Designar ícones únicos para cada tipo de carta e dado                     |
| C05 - Criar visuais distintos para cada item                              | F06 | Criar animações de aquisição e uso visual de cada item                    |
| C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F07 | Exibir dados coletados e regras do jogo no menu do "saco de dados"        |
| C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F08 | Implementar sistema de arrastar e soltar cartas no menu de deck           |
| C07 - Implementar sistema de lançamento de dados                          | F09 | Criar sistema de lançamento de dados com animação visual                  |
| C07 - Implementar sistema de lançamento de dados                          | F10 | Pegar o valor atual do dado no 3D e exibir resultado em HUD               |
| C08 - Implementar o sistema das cartas                                    | F11 | Implementar novos modificadores de cartas                                 |
| C09 - Gerar eventos com consequências variadas                            | F12 | Criar tabela de eventos com tipos: positivos, negativos e neutros         |
| C09 - Gerar eventos com consequências variadas                            | F13 | Escrever descrições e consequências únicas para cada evento               |
| C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F14 | Definir pontos de ativação para eventos aleatórios no mapa                |
| C11 - Gerar caminhos de progressão aleatórios entre níveis                | F15 | Gerar caminhos aleatórios conectando cenários                             |
| C11 - Gerar caminhos de progressão aleatórios entre níveis                | F16 | Definir pesos e condições para gerar as bifurcações                       |
| C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F17 | Implementar interação com o mapa                                          |
| C13 - Implementar interface de compra de cartas                           | F18 | Exibir loja com seções de cartas, dados e artefatos                       |
| C14 - Programar sistema de moedas e economia                              | F19 | Implementar sistema de moeda obtida em batalhas ou eventos                |
| C14 - Programar sistema de moedas e economia                              | F20 | Exibir saldo do jogador na interface durante o jogo                       |
| C15 - Criar estrutura de menus                                            | F21 | Criar menu de Pause                                                       |
| C15 - Criar estrutura de menus                                            | F22 | Criar menu de principal                                                   |
| C15 - Criar estrutura de menus                                            | F23 | Criar Opções do menu de Pause                                             |
| C16 - Implementar transições visuais entre menus                          | F24 | Adicionar transição de fase ao olhar para o mapa                          |
| C16 - Implementar transições visuais entre menus                          | F25 | Implementar sons de menu sincronizados com animações                      |
| C17 - Mostrar informações de combate e status do jogador                  | F26 | Exibir vida do jogador durante o combate (velas)                          |
| C17 - Mostrar informações de combate e status do jogador                  | F27 | Diminuir a iluminação conforme o jogador perde vida                       |
| C18 - Exibir efeitos visuais em ações como dano ou combo                  | F28 | Criar efeitos visuais de interação com objetos                            |
| C18 - Exibir efeitos visuais em ações como dano ou combo                  | F29 | Implementar os efeitos visuais de interação com objetos                   |
| C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F30 | Compor trilhas sonoras únicas para cada círculo com base em ambientação   |
| C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F31 | Mixar músicas em camadas (base, combate, tensão) para cada cenário        |
| C20 - Implementar variações dinâmicas na música conforme ações do jogador | F32 | Adicionar transições suaves entre trilhas com base em gatilhos do jogo    |
| C21 - Adicionar sons para interações, menus e ações de combate            | F33 |     Adicionar sons únicos para usos de carta e efeitos de combo           |
| C22 - Integrar efeitos sonoros com sistema de animação                    | F34 | Integrar sons dos NPCs                                                    |
| C27 - Escrever os diálogos do jogo                                        | F35 | Escrever diálogos para personagens importantes                            |
| C27 - Escrever os diálogos do jogo                                        | F36 | Organizar sistema de diálogo em planilha                                  |
| C28 - Implementar sistema de taunt de elites e boss para o jogador        | F37 | Criar falas provocativas para elites e chefes                             |
| C28 - Implementar sistema de taunt de elites e boss para o jogador        | F38 | Integrar sistema de taunts com entrada de combate do jogador              |
| C29 - Integrar o sistema de artefatos                                     | F39 | Criar o menu de artefatos                                                 |
| C29 - Integrar o sistema de artefatos                                     | F40 | Desbloquear os artefatos como colecionáveis                               |

## Priorização dos Itens do Backlog

A priorização dos itens do backlog foi baseada nos requisitos considerados mais relevantes. Os critérios utilizados foram:

- **Maior Importância**
- **Menor Complexidade**
- **Menor Risco & Incerteza**

Para determinar a prioridade de cada item, utilizou-se a seguinte fórmula:

**Prioridade = (2 * Importância) / 1 + ((2 * Risco&Incerteza) + Complexidade)**

Essa abordagem visa maximizar a entrega de valor, priorizando tarefas rápidas e impactantes. Com isso, buscamos garantir um progresso ágil e eficiente ao longo do desenvolvimento do jogo.

## Backlog Priorizado (WIP)

WIP

### Backlog - Desenvolvedores

| ID e Funcionalidade                                         | I | R&I | C | D | Prioridade |
|-------------------------------------------------------------|---|-----|---|---|------------|
| F08: Implementar sistema de arrastar e soltar cartas no menu de deck | 5 | 1   | 1 | 1 | ∞          |
| F09: Criar sistema de lançamento de dados com animação visual       | 5 | 1   | 1 | 1 | ∞          |
| F10: Pegar o valor atual do dado no 3D e exibir resultado em HUD    | 5 | 1   | 1 | 1 | ∞          |
| F11: Implementar novos modificadores de cartas                      | 5 | 1   | 1 | 1 | ∞          |
| F26: Exibir vida do jogador durante o combate (velas)              | 5 | 1   | 1 | 1 | **2.50**   |
| F07: Exibir dados coletados e regras no menu do "saco de dados"     | 5 | 1   | 1 | 1 | **2.50**   |
| F20: Exibir saldo do jogador na interface durante o jogo           | 5 | 1   | 1 | 1 | **2.50**   |
| F17: Implementar interação com o mapa                               | 5 | 1   | 1 | 2 | **1.25**   |
| F27: Diminuir a iluminação conforme o jogador perde vida           | 4 | 1   | 1 | 2 | **1.00**   |
| F14: Definir pontos de ativação para eventos aleatórios no mapa    | 5 | 3   | 5 | 1 | **0.83**   |
| F15: Gerar caminhos aleatórios conectando cenários                 | 5 | 3   | 5 | 1 | **0.83**   |
| F18: Exibir loja com cartas, dados e artefatos                     | 5 | 1   | 1 | 3 | **0.83**   |
| F21: Criar menu de pause                                           | 2 | 2   | 2 | 1 | **0.57**   |
| F39: Criar o menu de artefatos                                     | 1 | 1   | 1 | 1 | **0.50**   |
| F24: Adicionar transição de fase ao olhar para o mapa              | 2 | 1   | 1 | 2 | **0.50**   |
| F38: Integrar sistema de taunts com entrada de combate do jogador  | 3 | 2   | 2 | 2 | **0.43**   |
| F04: Integrar eventos de animação com sistema de combate           | 5 | 3   | 5 | 2 | **0.42**   |
| F29: Implementar os efeitos visuais de interação com objetos       | 2 | 1   | 2 | 3 | **0.27**   |
| F25: Implementar sons de menu sincronizados com animações          | 1 | 1   | 1 | 2 | **0.25**   |
| F34: Integrar sons dos NPCs                                        | 1 | 1   | 1 | 2 | **0.25**   |
| F40: Desbloquear os artefatos como colecionáveis                   | 1 | 1   | 1 | 2 | **0.25**   |
| F22: Criar menu principal                                          | 1 | 1   | 1 | 3 | **0.17**   |
| F23: Criar Opções do menu de Pause                                 | 2 | 4   | 5 | 2 | **0.14**   |
| F06: Criar animações de aquisição e uso visual de cada item        | 1 | 5   | 3 | 1 | **0.14**   |

### Backlog - Arte

| ID e Funcionalidade                                                     | I | R&I | C | D | Prioridade |
|-------------------------------------------------------------------------|---|-----|---|---|------------|
| F05: Designar ícones únicos para cada tipo de carta e dado (Em andamento) | 5 | 1   | 1 | 1 | ∞          |
| F02: Criar os sprites para os inimigos                                  | 5 | 2   | 3 | 1 | **0.63**   |
| F03: Criar os sprites para os NPCs                                      | 3 | 1   | 1 | 1 | **0.75**   |
| F01: Criar um fundo temático para cada círculo                          | 1 | 1   | 5 | 1 | **0.14**   |
| F28: Criar efeitos visuais de interação com objetos                     | 2 | 1   | 2 | 3 | **0.27**   |

### Backlog - Game Design

WIP

### Backlog - Música

WIP

### Backlog - Storytelling

WIP

---

## Histórico de Revisões
| Data       | Autor                                      | Alterações                                         |
| ---------- | ------------------------------------------ | -------------------------------------------------- |
| 2025-05-13 | [Mateus Vieira](https://github.com/matix0) | Reestruturação do backlog para maior consistência. |
| 2025-05-14 | [Mateus Vieira](https://github.com/matix0) | Criação do modelo SAFe sem o backlog final         |
| 2025-05-14 | [Mateus Vieira](https://github.com/matix0) | Backlog finalizado e priorizado                    |
| 2025-05-23 | [Vinícius Rufino](https://github.com/RufinoVfR) | Refatoração e Enriquecimento do Backlog         |
| 2025-05-27 | [Vinícius Rufino](https://github.com/RufinoVfR) | Refatoração e Correção das Funcionalidades         |
