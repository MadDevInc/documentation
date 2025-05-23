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
| C01 - Criar cenários únicos para cada círculo do Inferno                  | F02 | Integrar o cenário com objetos temáticos do círculo                       |
| C02 - Otimizar performance visual dos cenários                            | F03 | Definir aspectos técnicos referentes à performance                        |
| C02 - Otimizar performance visual dos cenários                            | F04 | Usar instâncias reutilizáveis para objetos do cenário                     |
| C03 - Criar modelos 2D para NPCs e inimigos                               | F05 | Criar os sprites para os inimigos                                         |
| C03 - Criar modelos 2D para NPCs e inimigos                               | F06 | Criar os sprites para os NPCs                                             |
| C04 - Integrar personagens com sistema de combate                         | F07 | Integrar eventos de animação com sistema de combate                       |
| C05 - Criar visuais distintos para cada item                              | F08 | Designar ícones únicos para cada tipo de carta e dado                     |
| C05 - Criar visuais distintos para cada item                              | F09 | Criar animações de aquisição e uso visual de cada item                    |
| C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F10 | Exibir dados coletados e regras do jogo no menu do "saco de dados"        |
| C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F11 | Implementar sistema de arrastar e soltar cartas no menu de deck           |
| C07 - Implementar sistema de lançamento de dados                          | F12 | Criar sistema de lançamento de dados com animação visual                  |
| C07 - Implementar sistema de lançamento de dados                          | F13 | Pegar o valor atual do dado no 3D e exibir resultado em HUD               |
| C08 - Implementar o sistema das cartas                                    | F14 | Implementar sistema de combos a partir das cartas                         |
| C08 - Implementar o sistema das cartas                                    | F15 | Aplicar efeitos específicos das cartas no inimigo ou jogador              |
| C09 - Gerar eventos com consequências variadas                            | F16 | Criar tabela de eventos com tipos: positivos, negativos e neutros         |
| C09 - Gerar eventos com consequências variadas                            | F17 | Escrever descrições e consequências únicas para cada evento               |
| C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F18 | Definir pontos de ativação para eventos aleatórios no mapa                |
| C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F19 | Integrar eventos aleatórios como interrupções no fluxo principal          |
| C11 - Gerar caminhos de progressão aleatórios entre níveis                | F20 | Gerar caminhos aleatórios conectando cenários com regras de progressão    |
| C11 - Gerar caminhos de progressão aleatórios entre níveis                | F21 | Definir pesos e condições para gerar as bifurcações                       |
| C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F22 | Criar mapa da trilha com visualização dos caminhos possíveis              |
| C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F23 | Permitir seleção de caminho com botão de confirmação                      |
| C13 - Implementar interface de compra de cartas                           | F24 | Exibir loja com seções de cartas disponíveis, raridade e custo            |
| C13 - Implementar interface de compra de cartas                           | F25 | Criar pop-up de confirmação de compra com descrição da carta              |
| C14 - Programar sistema de moedas e economia                              | F26 | Implementar sistema de moeda obtida em batalhas ou eventos                |
| C14 - Programar sistema de moedas e economia                              | F27 | Exibir saldo do jogador na interface da loja                              |
| C15 - Criar estrutura de menus                                            | F28 | Criar menus para: Jogo, Loja, Deck, Dados, Pausa, Configurações, Créditos |
| C15 - Criar estrutura de menus                                            | F29 | Programar navegação entre menus por teclado, mouse e controle             |
| C16 - Implementar transições visuais entre menus                          | F30 | Adicionar transições animadas entre menus                                 |
| C16 - Implementar transições visuais entre menus                          | F31 | Implementar sons de menu sincronizados com animações                      |
| C17 - Mostrar informações de combate e status do jogador                  | F32 | Exibir status do jogador (vida, cartas, dados) durante o combate          |
| C17 - Mostrar informações de combate e status do jogador                  | F33 | Exibir informações do inimigo                                             |
| C18 - Exibir efeitos visuais em ações como dano ou combo                  | F34 | Criar efeitos visuais de danos e combos                                   |
| C18 - Exibir efeitos visuais em ações como dano ou combo                  | F35 | Criar efeitos visuais de interação com objetos                            |
| C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F36 | Compor trilhas sonoras únicas para cada círculo com base em ambientação   |
| C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F37 | Mixar músicas em camadas (base, combate, tensão) para cada cenário        |
| C20 - Implementar variações dinâmicas na música conforme ações do jogador | F38 | Mudar a intensidade da trilha com base na ação do jogador (ex: combate)   |
| C20 - Implementar variações dinâmicas na música conforme ações do jogador | F39 | Adicionar transições suaves entre trilhas com base em gatilhos do jogo    |
| C21 - Adicionar sons para interações, menus e ações de combate            | F40 | Criar sons para interações e menus                                        |
| C21 - Adicionar sons para interações, menus e ações de combate            | F41 | Adicionar sons únicos para usos de carta e efeitos de combo               |
| C22 - Integrar efeitos sonoros com sistema de animação                    | F42 | Integrar sons com animações de ataque e interação                         |
| C22 - Integrar efeitos sonoros com sistema de animação                    | F43 | Integrar sons dos NPCs                                                    |
| C27 - Escrever os diálogos do jogo                                        | F44 | Escrever diálogos ramificados para personagens importantes                |
| C27 - Escrever os diálogos do jogo                                        | F45 | Organizar sistema de diálogo em planilha                                  |
| C28 - Implementar sistema de taunt de elites e boss para o jogador        | F46 | Criar falas provocativas para elites e chefes com base no combate         |
| C28 - Implementar sistema de taunt de elites e boss para o jogador        | F47 | Integrar sistema de taunts com entrada de combate do jogador              |
| C29 - Integrar o sistema de artefatos                                     | F48 | Criar o menu de artefatos                                                 |
| C29 - Integrar o sistema de artefatos                                     | F49 | Desbloquear os artefatos como colecionáveis                               |

## Backlog Priorizado (WIP)

Work In Progress

## Priorização dos Itens do Backlog

A priorização dos itens do backlog foi baseada nos requisitos considerados mais relevantes. Os critérios utilizados foram:

- **Maior Importância**
- **Menor Esforço**
- **Menor Risco**

Para determinar a prioridade de cada item, utilizou-se a seguinte fórmula:

**Prioridade = Importância / (Esforço + Risco)**

Essa abordagem visa maximizar a entrega de valor, priorizando tarefas rápidas e impactantes. Com isso, buscamos garantir um progresso ágil e eficiente ao longo do desenvolvimento do jogo.

---

## Histórico de Revisões
| Data       | Autor                                      | Alterações                                         |
| ---------- | ------------------------------------------ | -------------------------------------------------- |
| 2025-05-13 | [Mateus Vieira](https://github.com/matix0) | Reestruturação do backlog para maior consistência. |
| 2025-05-14 | [Mateus Vieira](https://github.com/matix0) | Criação do modelo SAFe sem o backlog final         |
| 2025-05-14 | [Mateus Vieira](https://github.com/matix0) | Backlog finalizado e priorizado                    |
| 2025-05-23 | [Vinícius Rufino](https://github.com/RufinoVfR) | Refatoração e Enriquecimento do Backlog         |
