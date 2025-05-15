# Backlog - Death Roll

## Estrutura do Backlog

| Categoria                                                 | Descrição                                                                                                                                                                     | Como Usar                                                                                                              |
| --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| [**Temas (TM)**](#temas-tm)                               | Representam as áreas principais do desenvolvimento do jogo, como Arte e Design, Jogabilidade, Interface do Usuário, Áudio e Trilha Sonora e Narrativa e Mundo.                | Escolha um tema para identificar a área de trabalho que será abordada (ex.: "Jogabilidade" para mecânicas de combate). |
| [**Épicos (EP)**](#epicos-ep)                             | São grandes blocos de trabalho dentro de cada tema. Eles descrevem objetivos amplos, como "Criação de Cenários" ou "Desenvolvimento de Mini-Games".                           | Divida o trabalho em épicos para organizar tarefas maiores dentro de cada tema.                                        |
| [**Capacidades (C)**](#capacidades-c)                     | Detalham os objetivos específicos de cada épico. Por exemplo, no épico "Combate", uma capacidade seria "Implementar mecânicas de lançamento de dados".                        | Use as capacidades para descrever o que precisa ser feito para alcançar o objetivo do épico.                           |
| [**Funcionalidades (F)**](#funcionalidades-f)             | São tarefas específicas que implementam as capacidades. Por exemplo, "Permitir que o jogador lance dados durante o combate".                                                  | Planeje e execute funcionalidades como tarefas individuais ou em sprints.                                              |
| [**Histórias de Usuário (US)**](#historias-de-usuario-us) | Detalham as interações do jogador com o sistema, sempre do ponto de vista do usuário. Por exemplo, "Como jogador, quero lançar dados para atacar inimigos durante o combate". | Use histórias de usuário para entender as necessidades do jogador e priorizar funcionalidades que entreguem valor.     |
| [**Histórico de Revisões**]()                             | Registra as alterações feitas no backlog, incluindo a data, o autor e uma breve descrição das mudanças.                                                                       | Consulte o histórico para acompanhar a evolução do backlog e manter a rastreabilidade.                                 |

## Temas (TM)

Os temas representam as áreas principais do desenvolvimento do jogo.

| ID   | Nome                  | Descrição                                                             |
| ---- | --------------------- | --------------------------------------------------------------------- |
| TM01 | Arte e Design         | Criação de cenários, personagens, itens e conceitos visuais.          |
| TM02 | Jogabilidade          | Desenvolvimento de mecânicas de combate, Eventos Aleatóriose eventos. |
| TM03 | Interface do Usuário  | Criação de menus e interações acessíveis e intuitivas.                |
| TM04 | Áudio e Trilha Sonora | Composição de músicas e efeitos sonoros imersivos.                    |
| TM05 | Narrativa e Mundo     | Construção da história, ambientação e progressão do jogador.          |

---

## Épicos (EP)

Os épicos são grandes blocos de trabalho dentro de cada tema.

| ID   | Tema                  | Nome                   | Descrição                                                                                    |
| ---- | --------------------- | ---------------------- | -------------------------------------------------------------------------------------------- |
| EP01 | Arte e Design         | Criação de Cenários    | Desenvolvimento de 9 cenários distintos para o jogo.                                         |
| EP02 | Arte e Design         | Criação de Personagens | Modelagem de inimigos, NPCs e outros elementos visuais.                                      |
| EP03 | Arte e Design         | Design de Itens        | Criação de dados, cartas, baús e outros objetos.                                             |
| EP04 | Jogabilidade          | Combate                | Desenvolvimento de mecânicas de combate baseadas em dados e cartas.                          |
| EP05 | Jogabilidade          | Eventos Aleatórios     | Implementação de Eventos Aleatórios                                                          |
| EP06 | Jogabilidade          | Sistema de Trilha      | Criação de mecânicas de progressão de níveis com escolha de caminhos aleatóriamente gerados. |
| EP07 | Jogabilidade          | Loja                   | Criação de uma loja para compra de cartas                                                    |
| EP08 | Interface do Usuário  | Menus de Navegação     | Criação de menus para loja, deck, dados, pausa e diálogo.                                    |
| EP09 | Interface do Usuário  | HUD e Feedback Visual  | Desenvolvimento de elementos visuais para exibir informações ao jogador.                     |
| EP10 | Áudio e Trilha Sonora | Composição de Músicas  | Criação de trilhas sonoras temáticas para cada círculo do Inferno.                           |
| EP11 | Áudio e Trilha Sonora | Efeitos Sonoros        | Desenvolvimento de sons para ações e ambientação.                                            |
| EP12 | Narrativa e Mundo     | Diálogos               | Criação dos diálogos do jogo.                                                                |

---

## Capacidades (C)

As capacidades detalham os objetivos específicos de cada épico.

| ID  | Épico                         | Capacidade                                                          |
| --- | ----------------------------- | ------------------------------------------------------------------- |
| C01 | EP01 - Criação de Cenários    | Criar cenários únicos para cada círculo do Inferno                  |
| C02 | EP01 - Criação de Cenários    | Otimizar performance visual dos cenários                            |
| C03 | EP02 - Criação de Personagens | Criar modelos 2D para NPCs e inimigos                               |
| C04 | EP02 - Criação de Personagens | Integrar personagens com sistema de combate                         |
| C05 | EP03 - Design de Itens        | Criar visuais distintos para cada item                              |
| C06 | EP03 - Design de Itens        | Integrar itens com sistema de menu (saco de dados e deck)           |
| C07 | EP04 - Combate                | Implementar sistema de lançamento de dados                          |
| C08 | EP04 - Combate                | Implementar o sistema das cartas                                    |
| C09 | EP05 - Eventos Aleatórios     | Gerar eventos com consequências variadas                            |
| C10 | EP05 - Eventos Aleatórios     | Integrar eventos aleatórios ao fluxo de gameplay                    |
| C11 | EP06 - Sistema de Trilha      | Gerar caminhos de progressão aleatórios entre níveis                |
| C12 | EP06 - Sistema de Trilha      | Exibir mapa da trilha com opções de escolha visíveis ao jogador     |
| C13 | EP07 - Loja                   | Implementar interface de compra de cartas                           |
| C14 | EP07 - Loja                   | Programar sistema de moedas e economia                              |
| C15 | EP08 - Menus de Navegação     | Criar estrutura de menus                                            |
| C16 | EP08 - Menus de Navegação     | Implementar transições visuais entre menus                          |
| C17 | EP09 - HUD e Feedback Visual  | Mostrar informações de combate e status do jogador                  |
| C18 | EP09 - HUD e Feedback Visual  | Exibir efeitos visuais em ações como dano ou combo                  |
| C19 | EP10 - Composição de Músicas  | Criar trilhas sonoras adaptadas a cada círculo do Inferno           |
| C20 | EP10 - Composição de Músicas  | Implementar variações dinâmicas na música conforme ações do jogador |
| C21 | EP11 - Efeitos Sonoros        | Adicionar sons para interações, menus e ações de combate            |
| C22 | EP11 - Efeitos Sonoros        | Integrar efeitos sonoros com sistema de animação                    |
| C27 | EP14 - Diálogos               | Escrever os diálogos do jogo                                        |
| C28 | EP14 - Diálogos               | Implementar sistema de taunt de elites e boss para o jogador        |
| C29 | EP03 - Design de Itens        | Integrar o sistema de artefatos                                     |

## Funcionalidades (F)

As funcionalidades são tarefas específicas que implementam as capacidades.

| ID  | Capacidade (ID + Nome)                                                    | Funcionalidade                                                            |
| --- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| F01 | C01 - Criar cenários únicos para cada círculo do Inferno                  | Criar um fundo temático para cada círculo                                 |
| F02 | C01 - Criar cenários únicos para cada círculo do Inferno                  | Integrar o cenário com objetos temáticos do círculo                       |
| F03 | C02 - Otimizar performance visual dos cenários                            | Definir aspectos técnicos referentes à performance                        |
| F04 | C02 - Otimizar performance visual dos cenários                            | Usar instâncias reutilizáveis para objetos do cenário                     |
| F05 | C03 - Criar modelos 2D para NPCs e inimigos                               | Criar os sprites para os inimigos                                         |
| F06 | C03 - Criar modelos 2D para NPCs e inimigos                               | Criar os sprites para os NPCs                                             |
| F07 | C04 - Integrar personagens com sistema de combate                         | Integrar eventos de animação com sistema de combate                       |
| F08 | C05 - Criar visuais distintos para cada item                              | Designar ícones únicos para cada tipo de carta e dado                     |
| F09 | C05 - Criar visuais distintos para cada item                              | Criar animações de aquisição e uso visual de cada item                    |
| F10 | C06 - Integrar itens com sistema de menu (saco de dados e deck)           | Exibir dados coletados e regras do jogo no menu do "saco de dados"        |
| F11 | C06 - Integrar itens com sistema de menu (saco de dados e deck)           | Implementar sistema de arrastar e soltar cartas no menu de deck           |
| F12 | C07 - Implementar sistema de lançamento de dados                          | Criar sistema de lançamento de dados com animação visual                  |
| F13 | C07 - Implementar sistema de lançamento de dados                          | Pegar o valor atual do dado no 3D e exibir resultado em HUD               |
| F14 | C08 - Implementar o sistema das cartas                                    | Implementar sistema de combos a partir das cartas                         |
| F15 | C08 - Implementar o sistema das cartas                                    | Aplicar efeitos específicos das cartas no inimigo ou jogador              |
| F16 | C09 - Gerar eventos com consequências variadas                            | Criar tabela de eventos com tipos: positivos, negativos e neutros         |
| F17 | C09 - Gerar eventos com consequências variadas                            | Escrever descrições e consequências únicas para cada evento               |
| F18 | C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | Definir pontos de ativação para eventos aleatórios no mapa                |
| F19 | C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | Integrar eventos aleatórios como interrupções no fluxo principal          |
| F20 | C11 - Gerar caminhos de progressão aleatórios entre níveis                | Gerar caminhos aleatórios conectando cenários com regras de progressão    |
| F21 | C11 - Gerar caminhos de progressão aleatórios entre níveis                | Definir pesos e condições para gerar as bifurcações                       |
| F22 | C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | Criar mapa da trilha com visualização dos caminhos possíveis              |
| F23 | C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | Permitir seleção de caminho com botão de confirmação                      |
| F24 | C13 - Implementar interface de compra de cartas                           | Exibir loja com seções de cartas disponíveis, raridade e custo            |
| F25 | C13 - Implementar interface de compra de cartas                           | Criar pop-up de confirmação de compra com descrição da carta              |
| F26 | C14 - Programar sistema de moedas e economia                              | Implementar sistema de moeda obtida em batalhas ou eventos                |
| F27 | C14 - Programar sistema de moedas e economia                              | Exibir saldo do jogador na interface da loja                              |
| F28 | C15 - Criar estrutura de menus                                            | Criar menus para: Jogo, Loja, Deck, Dados, Pausa, Configurações, Créditos |
| F29 | C15 - Criar estrutura de menus                                            | Programar navegação entre menus por teclado, mouse e controle             |
| F30 | C16 - Implementar transições visuais entre menus                          | Adicionar transições animadas entre menus                                 |
| F31 | C16 - Implementar transições visuais entre menus                          | Implementar sons de menu sincronizados com animações                      |
| F32 | C17 - Mostrar informações de combate e status do jogador                  | Exibir status do jogador (vida, cartas, dados) durante o combate          |
| F33 | C17 - Mostrar informações de combate e status do jogador                  | Exibir informações do inimigo                                             |
| F34 | C18 - Exibir efeitos visuais em ações como dano ou combo                  | Criar efeitos visuais de danos e combos                                   |
| F35 | C18 - Exibir efeitos visuais em ações como dano ou combo                  | Criar efeitos visuais de interação com objetos                            |
| F36 | C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | Compor trilhas sonoras únicas para cada círculo com base em ambientação   |
| F37 | C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | Mixar músicas em camadas (base, combate, tensão) para cada cenário        |
| F38 | C20 - Implementar variações dinâmicas na música conforme ações do jogador | Mudar a intensidade da trilha com base na ação do jogador (ex: combate)   |
| F39 | C20 - Implementar variações dinâmicas na música conforme ações do jogador | Adicionar transições suaves entre trilhas com base em gatilhos do jogo    |
| F40 | C21 - Adicionar sons para interações, menus e ações de combate            | Criar sons para interações e menus                                        |
| F41 | C21 - Adicionar sons para interações, menus e ações de combate            | Adicionar sons únicos para usos de carta e efeitos de combo               |
| F42 | C22 - Integrar efeitos sonoros com sistema de animação                    | Integrar sons com animações de ataque e interação                         |
| F43 | C22 - Integrar efeitos sonoros com sistema de animação                    | Integrar sons dos NPCs                                                    |
| F44 | C27 - Escrever os diálogos do jogo                                        | Escrever diálogos ramificados para personagens importantes                |
| F45 | C27 - Escrever os diálogos do jogo                                        | Organizar sistema de diálogo em planilha                                  |
| F46 | C28 - Implementar sistema de taunt de elites e boss para o jogador        | Criar falas provocativas para elites e chefes com base no combate         |
| F47 | C28 - Implementar sistema de taunt de elites e boss para o jogador        | Integrar sistema de taunts com entrada de combate do jogador              |
| F48 | C29 - Integrar o sistema de artefatos                                     | Criar o menu de artefatos                                                 |
| F49 | C29 - Integrar o sistema de artefatos                                     | Desbloquear os artefatos como colecionáveis                               |

---

## Histórias de Usuário (US)

As histórias de usuário detalham as interações do jogador com o sistema.

| ID   | Funcionalidade (ID + Nome)                      | História de Usuário (US)                                                                                              |
| ---- | ----------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| US01 | F01 - Criar um fundo temático para cada círculo | Como jogador, quero visualizar cenários únicos em cada círculo do Inferno para imersão na ambientação.                |
| US02 | F01 - Criar um fundo temático para cada círculo | Como artista, quero criar assets visuais distintos para cada círculo que reflitam suas características temáticas.     |
| US03 | F02 - Integrar cenário com objetos temáticos    | Como jogador, quero visualizar objetos ambientais que complementem a narrativa de cada círculo.                       |
| US04 | F02 - Integrar cenário com objetos temáticos    | Como artista, quero criar entidades para o cenário com interações consistentes com a jogabilidade.                    |
| US05 | F03 - Definir aspectos técnicos de performance  | Como desenvolvedor, quero otimizar polígonos e texturas para manter uma taxa estável de FPS                           |
| US06 | F03 - Definir aspectos técnicos de performance  | Como jogador, quero uma experiência fluida sem travamentos durante transições de cenário.                             |
| US07 | F04 - Usar instâncias reutilizáveis             | Como desenvolvedor, quero reutilizar assets de cenário com variações para reduzir carga de memória.                   |
| US08 | F05 - Criar sprites para inimigos               | Como jogador, quero identificar visualmente tipos de inimigos por seus designs únicos.                                |
| US09 | F05 - Criar sprites para inimigos               | Como artista, quero criar sprites que comuniquem claramente a raridade e periculosidade de cada inimigo.              |
| US10 | F06 - Criar sprites para NPCs                   | Como jogador, quero reconhecer NPCs importantes por seus designs distintivos.                                         |
| US11 | F06 - Criar sprites para NPCs                   | Como narrador, quero que NPCs tenham expressões faciais variadas para enriquecer diálogos.                            |
| US12 | F07 - Integrar animações com combate            | Como jogador, quero ver animações fluidas durante ataques e defesas no combate.                                       |
| US13 | F07 - Integrar animações com combate            | Como desenvolvedor, quero sincronizar eventos de animação com triggers do sistema de combate.                         |
| US14 | F08 - Designar ícones para cartas e dados       | Como jogador, quero identificar rapidamente tipos de cartas/dados por seus ícones durante o combate.                  |
| US15 | F08 - Designar ícones para cartas e dados       | Como artista, quero criar ícones que sigam uma sinalização consistente por raridade.                                  |
| US16 | F09 - Criar animações de aquisição de itens     | Como jogador, quero ver feedback visual ao adquirir novos itens .                                                     |
| US17 | F09 - Criar animações de aquisição de itens     | Como desenvolvedor, quero que animações de itens não interrompam o fluxo do jogo.                                     |
| US18 | F10 - Exibir dados coletados no menu            | Como jogador, quero consultar regras e estatísticas dos meus dados a qualquer momento.                                |
| US19 | F10 - Exibir dados coletados no menu            | Como desenvolvedor, quero organizar as informações do saco de dados em categorias intuitivas.                         |
| US20 | F11 - Implementar arrastar/soltar cartas        | Como jogador, quero reorganizar meu deck arrastando cartas com o mouse/controle.                                      |
| US21 | F11 - Implementar arrastar/soltar cartas        | Como UX designer, quero fornecer feedback visual durante a interação de arrastar (hover, drop válido/inválido).       |
| US22 | F12 - Criar sistema de lançamento de dados      | Como jogador, quero lançar dados com física realista e resultados claramente visíveis.                                |
| US23 | F12 - Criar sistema de lançamento de dados      | Como desenvolvedor, quero calcular resultados com base na posição final do dado 3D.                                   |
| US24 | F13 - Exibir resultado do dado no HUD           | Como jogador, quero ver imediatamente o valor do dado em uma interface clara durante o combate.                       |
| US25 | F13 - Exibir resultado do dado no HUD           | Como desenvolvedor, quero formatar a exibição do resultado para ser legível em diferentes resoluções.                 |
| US26 | F14 - Implementar sistema de combos             | Como jogador, quero executar combos específicos ao jogar sequências de cartas para efeitos.                           |
| US27 | F14 - Implementar sistema de combos             | Como game designer, quero criar um sistema de combos para dados.                                                      |
| US28 | F15 - Aplicar efeitos de cartas                 | Como jogador, quero ver feedback visual claro quando efeitos de cartas são ativados (positivos/negativos).            |
| US29 | F15 - Aplicar efeitos de cartas                 | Como desenvolvedor, quero implementar um sistema modular de efeitos que possa ser expandido com novas cartas.         |
| US30 | F16 - Criar tabela de eventos                   | Como game designer, quero criar eventos com probabilidades balanceadas para evitar repetição excessiva.               |
| US31 | F16 - Criar tabela de eventos                   | Como jogador, quero encontrar eventos aleatórios para me beneficiar (ou não) em jogo.                                 |
| US32 | F17 - Escrever descrições de eventos            | Como narrador, quero que eventos tenham textos imersivos que complementem o tom do jogo.                              |
| US33 | F17 - Escrever descrições de eventos            | Como jogador, quero entender claramente as consequências de minhas escolhas nos eventos.                              |
| US34 | F18 - Definir pontos de ativação                | Como designer, quero distribuir eventos aleatórios de forma a manter um ritmo de jogo equilibrado.                    |
| US35 | F18 - Definir pontos de ativação                | Como jogador, quero poder selecionar o evento aleatório na trilha.                                                    |
| US36 | F19 - Integrar eventos como interrupções        | Como jogador, quero que eventos aleatórios ofereçam pausas estratégicas no fluxo principal.                           |
| US37 | F19 - Integrar eventos como interrupções        | Como desenvolvedor, quero implementar um sistema que garanta que eventos não travem o progresso principal.            |
| US38 | F20 - Gerar caminhos aleatórios                 | Como jogador, quero utilizar um sistema de navegação em trilha aleatório                                              |
| US39 | F20 - Gerar caminhos aleatórios                 | Como desenvolvedor, quero garantir que caminhos sejam gerados aleatóriamente.                                         |
| US40 | F21 - Definir pesos para bifurcações            | Como game designer, quero controlar a probabilidade de certos tipos de encontros aparecerem em cada nível.            |
| US41 | F21 - Definir pesos para bifurcações            | Como jogador, quero sentir um senso de escolha e análise a partir das bifurcações.                                    |
| US42 | F22 - Criar mapa da trilha                      | Como jogador, quero visualizar meu progresso e opções futuras no mapa de forma intuitiva.                             |
| US43 | F22 - Criar mapa da trilha                      | Como UX designer, quero representar visualmente os tipos de encontros possíveis em cada nó do mapa.                   |
| US44 | F23 - Permitir seleção de caminho               | Como jogador, quero confirmar minha escolha de caminho antes de prosseguir para evitar erros.                         |
| US45 | F23 - Permitir seleção de caminho               | Como desenvolvedor, quero implementar um fluxo para ser seguido pelo jogador                                          |
| US46 | F24 - Exibir loja com cartas disponíveis        | Como jogador, quero visualizar estatísticas e custos das cartas antes de comprar.                                     |
| US47 | F24 - Exibir loja com cartas disponíveis        | Como desenvolvedor, quero realizar uma tabela de possibilidades para aquisição das cartas                             |
| US48 | F25 - Criar pop-up de confirmação               | Como jogador, quero ver detalhes completos da carta antes de confirmar a compra.                                      |
| US49 | F25 - Criar pop-up de confirmação               | Como UX designer, quero evitar compras acidentais com confirmação clara mas não intrusiva.                            |
| US50 | F26 - Implementar sistema de moeda              | Como jogador, quero ganhar moedas de forma proporcional ao desafio superado.                                          |
| US51 | F26 - Implementar sistema de moeda              | Como designer, quero balancear a economia para que moedas sejam valiosas mas não excessivamente raras.                |
| US52 | F27 - Exibir saldo na loja                      | Como jogador, quero ver meu saldo atualizado em tempo real durante compras.                                           |
| US53 | F27 - Exibir saldo na loja                      | Como desenvolvedor, quero formatar a exibição de moedas para ser legível mesmo em valores altos.                      |
| US54 | F28 - Criar menus principais                    | Como jogador, quero acessar todas as funcionalidades principais em no máximo 3 cliques a partir do menu inicial.      |
| US55 | F28 - Criar menus principais                    | Como desenvolvedor, quero implementar um sistema de navegação por teclado/controle seguindo padrões acessíveis.       |
| US56 | F29 - Programar navegação entre menus           | Como jogador, quero navegar os menus usando atalhos intuitivos (setas, Enter, Esc).                                   |
| US57 | F29 - Programar navegação entre menus           | Como testador, quero garantir que o foco do controle nunca se perda durante a navegação.                              |
| US58 | F30 - Adicionar transições animadas             | Como jogador, quero transições suaves entre menus que não causem desorientação.                                       |
| US59 | F30 - Adicionar transições animadas             | Como desenvolvedor, quero otimizar animações para que não aumentem significativamente o tempo de carregamento.        |
| US60 | F31 - Implementar sons de menu                  | Como jogador, quero feedback auditivo claro para interações com menus.                                                |
| US61 | F31 - Implementar sons de menu                  | Como designer de som, quero criar uma identidade auditiva consistente para todas as interfaces.                       |
| US62 | F32 - Exibir status do jogador                  | Como jogador, quero monitorar minha vida, recursos e status atual durante o combate sem obstruir a visão.             |
| US63 | F32 - Exibir status do jogador                  | Como UX designer, quero organizar as informações prioritárias no HUD de forma hierárquica.                            |
| US64 | F33 - Exibir informações do inimigo             | Como jogador, quero ver a vida e status dos inimigos para planejar minha estratégia.                                  |
| US65 | F33 - Exibir informações do inimigo             | Como desenvolvedor, quero implementar um sistema de barras de vida que escalone para diferentes tamanhos de inimigos. |
| US66 | F34 - Criar efeitos visuais de dano             | Como jogador, quero feedback visual imediato quando causo ou recebo dano.                                             |
| US67 | F34 - Criar efeitos visuais de dano             | Como artista, quero diferenciar visualmente tipos de dano (inimigo, jogador)                                          |
| US68 | F35 - Criar efeitos de interação                | Como jogador, quero perceber claramente quando um objeto no cenário é interagível.                                    |
| US69 | F35 - Criar efeitos de interação                | Como desenvolvedor, quero que efeitos de interação não sobrecarreguem visualmente o jogador.                          |
| US70 | F36 - Compor trilhas para cada círculo          | Como jogador, quero músicas que reforcem a identidade única de cada círculo do Inferno.                               |
| US71 | F36 - Compor trilhas para cada círculo          | Como compositor, quero criar leitmotivs que evoluam conforme o jogador progride.                                      |
| US72 | F37 - Mixar músicas em camadas                  | Como jogador, quero transições dinâmicas entre estados musicais (mapa -> combate).                                    |
| US73 | F37 - Mixar músicas em camadas                  | Como desenvolvedor, quero um sistema que alterne entre camadas musicais sem cortes ou repetições bruscas.             |
| US74 | F38 - Mudar intensidade da trilha               | Como jogador, quero que a música reflita a tensão do momento (ex: chefes finais tenham trilhas épicas).               |
| US75 | F38 - Mudar intensidade da trilha               | Como designer de áudio, quero implementar parâmetros dinâmicos que modifiquem a música com base no estado do jogo.    |
| US76 | F39 - Adicionar transições entre trilhas        | Como jogador, quero transições musicais suaves ao mudar de área ou entrar em combate.                                 |
| US77 | F39 - Adicionar transições entre trilhas        | Como desenvolvedor, quero garantir que transições musicais não causem stuttering ou lag.                              |
| US78 | F40 - Criar sons para interações                | Como jogador, quero feedback auditivo único para ações importantes.                                                   |
| US79 | F40 - Criar sons para interações                | Como designer de som, quero estabelecer uma paleta sonora coerente com o tema sombrio do jogo.                        |
| US80 | F41 - Adicionar sons de cartas                  | Como jogador, quero sons distintos para cartas de diferentes raridades.                                               |
| US81 | F41 - Adicionar sons de cartas                  | Como desenvolvedor, quero que sons de cartas sejam espacializados quando aplicável.                                   |
| US82 | F42 - Integrar sons com animações               | Como jogador, quero sincronia perfeita entre sons e animações de ataques.                                             |
| US83 | F42 - Integrar sons com animações               | Como animador, quero marcas temporais precisas para sincronizar efeitos sonoros.                                      |
| US84 | F43 - Integrar sons dos NPCs                    | Como jogador, quero que NPCs tenham vozes ou sons característicos que os diferenciem.                                 |
| US85 | F43 - Integrar sons dos NPCs                    | Como desenvolvedor, quero que diálogos importantes tenham prioridade sonora sobre ambientes.                          |
| US86 | F44 - Escrever diálogos ramificados             | Como jogador, quero que minhas escolhas nos diálogos impactem a narrativa e o mundo.                                  |
| US87 | F44 - Escrever diálogos ramificados             | Como escritor, quero estruturar diálogos em árvores lógicas que sejam fáceis de implementar.                          |
| US88 | F45 - Organizar diálogos em planilha            | Como desenvolvedor, quero exportar diálogos para o engine a partir de planilhas.                                      |
| US89 | F45 - Organizar diálogos em planilha            | Como tradutor, quero acesso estruturado a todos os textos do jogo para tradução.                                      |
| US90 | F46 - Criar falas provocativas                  | Como jogador, quero que chefes reajam às minhas ações durante o combate com falas imersivas.                          |
| US91 | F46 - Criar falas provocativas                  | Como escritor, quero criar taunts que variem conforme a progressão do jogador no combate.                             |
| US92 | F47 - Integrar taunts com combate               | Como jogador, quero que provocações de chefes sejam acionadas em momentos dramáticos (ex: baixa vida, combos).        |
| US93 | F47 - Integrar taunts com combate               | Como desenvolvedor, quero implementar um sistema de triggers que não interrompa o fluxo do combate.                   |
| US94 | F48 - Criar menu de artefatos                   | Como jogador, quero visualizar minha coleção de artefatos.                                                            |
| US95 | F48 - Criar menu de artefatos                   | Como designer, quero que o menu de artefatos mostre progresso de conquistas relacionadas.                             |
| US96 | F49 - Desbloquear artefatos colecionáveis       | Como jogador, quero receber artefatos como recompensa por desafios significativos.                                    |
| US97 | F49 - Desbloquear artefatos colecionáveis       | Como desenvolvedor, quero rastrear artefatos desbloqueados via sistema de save.                                       |

---

## Histórias de Usuário Priorizadas

| US  | Complexidade | Risco | Importância | Valor Priorizado |
| --- | ------------ | ----- | ----------- | ---------------- |
| 29  | 4            | 1     | 5           | 20               |
| 51  | 4            | 1     | 5           | 20               |
| 60  | 4            | 1     | 5           | 20               |
| 69  | 4            | 1     | 5           | 20               |
| 79  | 4            | 1     | 5           | 20               |
| 8   | 3            | 1     | 5           | 15               |
| 9   | 3            | 1     | 5           | 15               |
| 10  | 3            | 1     | 5           | 15               |
| 14  | 3            | 1     | 5           | 15               |
| 28  | 3            | 1     | 5           | 15               |
| 31  | 3            | 1     | 5           | 15               |
| 50  | 3            | 1     | 5           | 15               |
| 63  | 3            | 1     | 5           | 15               |
| 68  | 3            | 1     | 5           | 15               |
| 87  | 3            | 1     | 5           | 15               |
| 38  | 5            | 2     | 5           | 12.5             |
| 61  | 5            | 2     | 5           | 12.5             |
| 90  | 4            | 2     | 5           | 10               |
| 12  | 2            | 1     | 5           | 10               |
| 18  | 2            | 1     | 5           | 10               |
| 25  | 2            | 1     | 5           | 10               |
| 42  | 2            | 1     | 5           | 10               |
| 43  | 2            | 1     | 5           | 10               |
| 46  | 2            | 1     | 5           | 10               |
| 48  | 2            | 1     | 5           | 10               |
| 49  | 2            | 1     | 5           | 10               |
| 62  | 2            | 1     | 5           | 10               |
| 64  | 2            | 1     | 5           | 10               |
| 66  | 2            | 1     | 5           | 10               |
| 89  | 2            | 1     | 5           | 10               |
| 91  | 2            | 1     | 5           | 10               |
| 26  | 3            | 2     | 5           | 7.5              |
| 36  | 3            | 2     | 5           | 7.5              |
| 37  | 3            | 2     | 5           | 7.5              |
| 27  | 4            | 3     | 5           | 6.666666667      |
| 30  | 4            | 3     | 5           | 6.666666667      |
| 34  | 4            | 3     | 5           | 6.666666667      |
| 45  | 5            | 5     | 5           | 5                |
| 17  | 3            | 3     | 5           | 5                |
| 39  | 3            | 3     | 5           | 5                |
| 93  | 3            | 3     | 5           | 5                |
| 22  | 1            | 1     | 5           | 5                |
| 23  | 1            | 1     | 5           | 5                |
| 24  | 1            | 1     | 5           | 5                |
| 32  | 1            | 1     | 5           | 5                |
| 33  | 1            | 1     | 5           | 5                |
| 35  | 1            | 1     | 5           | 5                |
| 44  | 1            | 1     | 5           | 5                |
| 52  | 1            | 1     | 5           | 5                |
| 88  | 1            | 1     | 5           | 5                |
| 13  | 2            | 3     | 5           | 3.333333333      |
| 41  | 3            | 5     | 5           | 3                |
| 84  | 4            | 1     | 4           | 16               |
| 92  | 4            | 1     | 4           | 16               |
| 15  | 3            | 1     | 4           | 12               |
| 16  | 3            | 1     | 4           | 12               |
| 47  | 3            | 1     | 4           | 12               |
| 65  | 3            | 1     | 4           | 12               |
| 70  | 3            | 1     | 4           | 12               |
| 76  | 3            | 1     | 4           | 12               |
| 78  | 3            | 1     | 4           | 12               |
| 82  | 3            | 1     | 4           | 12               |
| 58  | 2            | 1     | 4           | 8                |
| 83  | 3            | 2     | 4           | 6                |
| 40  | 1            | 1     | 4           | 4                |
| 54  | 1            | 1     | 4           | 4                |
| 74  | 4            | 1     | 3           | 12               |
| 20  | 3            | 1     | 3           | 9                |
| 21  | 3            | 1     | 3           | 9                |
| 59  | 3            | 1     | 3           | 9                |
| 67  | 3            | 1     | 3           | 9                |
| 86  | 3            | 1     | 3           | 9                |
| 94  | 2            | 1     | 3           | 6                |
| 95  | 2            | 1     | 3           | 6                |
| 96  | 2            | 1     | 3           | 6                |
| 97  | 2            | 1     | 3           | 6                |
| 55  | 3            | 2     | 3           | 4.5              |
| 56  | 3            | 2     | 3           | 4.5              |
| 57  | 3            | 2     | 3           | 4.5              |
| 77  | 3            | 3     | 3           | 3                |
| 71  | 5            | 1     | 2           | 10               |
| 73  | 5            | 1     | 2           | 10               |
| 85  | 2            | 1     | 2           | 4                |
| 11  | 5            | 4     | 2           | 2.5              |
| 7   | 1            | 1     | 2           | 2                |
| 53  | 1            | 1     | 2           | 2                |
| 4   | 4            | 1     | 1           | 4                |
| 72  | 4            | 1     | 1           | 4                |
| 75  | 4            | 1     | 1           | 4                |
| 1   | 3            | 1     | 1           | 3                |
| 2   | 3            | 1     | 1           | 3                |
| 3   | 3            | 1     | 1           | 3                |
| 80  | 2            | 1     | 1           | 2                |
| 5   | 5            | 5     | 1           | 1                |
| 6   | 5            | 5     | 1           | 1                |
| 19  | 1            | 1     | 1           | 1                |
| 81  | 1            | 1     | 1           | 1                |

## Backlog Priorizado
 | **Tema (tm-xx)** | **Épico (Ep-xx)**             | **Capacidade (C)**                                                        | **Funcionalidade (F)**                                                          | **História de usuário (US)**                                                                                                 | **Valor Priorizado (VP)** |
 | ---------------- | ----------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------- |
 | TM02             | EP04 - Combate                | C08 - Implementar o sistema das cartas                                    | F15 - Aplicar efeitos específicos das cartas no inimigo ou jogador              | US29 - Como desenvolvedor, quero implementar um sistema modular de efeitos que possa ser expandido com novas cartas.         | 20                        |
 | TM02             | EP07 - Loja                   | C14 - Programar sistema de moedas e economia                              | F26 - Implementar sistema de moeda obtida em batalhas ou eventos                | US51 - Como designer, quero balancear a economia para que moedas sejam valiosas mas não excessivamente raras.                | 20                        |
 | TM03             | EP08 - Menus de Navegação     | C16 - Implementar transições visuais entre menus                          | F31 - Implementar sons de menu sincronizados com animações                      | US60 - Como jogador, quero feedback auditivo claro para interações com menus.                                                | 20                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C18 - Exibir efeitos visuais em ações como dano ou combo                  | F35 - Criar efeitos visuais de interação com objetos                            | US69 - Como desenvolvedor, quero que efeitos de interação não sobrecarreguem visualmente o jogador.                          | 20                        |
 | TM04             | EP11 - Efeitos Sonoros        | C21 - Adicionar sons para interações, menus e ações de combate            | F40 - Criar sons para interações e menus                                        | US79 - Como designer de som, quero estabelecer uma paleta sonora coerente com o tema sombrio do jogo.                        | 20                        |
 | TM04             | EP11 - Efeitos Sonoros        | C22 - Integrar efeitos sonoros com sistema de animação                    | F43 - Integrar sons dos NPCs                                                    | US84 - Como jogador, quero que NPCs tenham vozes ou sons característicos que os diferenciem.                                 | 16                        |
 | TM05             | EP12 - Diálogos               | C28 - Implementar sistema de taunt de elites e boss para o jogador        | F47 - Integrar sistema de taunts com entrada de combate do jogador              | US92 - Como jogador, quero que provocações de chefes sejam acionadas em momentos dramáticos (ex: baixa vida, combos).        | 16                        |
 | TM01             | EP01 - Criação de Cenários    | C01 - Criar cenários únicos para cada círculo do Inferno                  | F01 - Criar um fundo temático para cada círculo                                 | US01 - Como jogador, quero visualizar cenários únicos em cada círculo do Inferno para imersão na ambientação.                | 15                        |
 | TM01             | EP01 - Criação de Cenários    | C01 - Criar cenários únicos para cada círculo do Inferno                  | F01 - Criar um fundo temático para cada círculo                                 | US02 - Como artista, quero criar assets visuais distintos para cada círculo que reflitam suas características temáticas.     | 15                        |
 | TM01             | EP01 - Criação de Cenários    | C01 - Criar cenários únicos para cada círculo do Inferno                  | F02 - Integrar cenário com objetos temáticos                                    | US03 - Como jogador, quero visualizar objetos ambientais que complementem a narrativa de cada círculo.                       | 15                        |
 | TM01             | EP01 - Criação de Cenários    | C01 - Criar cenários únicos para cada círculo do Inferno                  | F02 - Integrar cenário com objetos temáticos                                    | US04 - Como artista, quero criar entidades para o cenário com interações consistentes com a jogabilidade.                    | 15                        |
 | TM01             | EP02 - Criação de Personagens | C03 - Criar modelos 2D para NPCs e inimigos                               | F05 - Criar os sprites para os inimigos                                         | US08 - Como jogador, quero identificar visualmente tipos de inimigos por seus designs únicos.                                | 15                        |
 | TM01             | EP02 - Criação de Personagens | C03 - Criar modelos 2D para NPCs e inimigos                               | F05 - Criar os sprites para os inimigos                                         | US09 - Como artista, quero criar sprites que comuniquem claramente a raridade e periculosidade de cada inimigo.              | 15                        |
 | TM01             | EP02 - Criação de Personagens | C03 - Criar modelos 2D para NPCs e inimigos                               | F06 - Criar os sprites para os NPCs                                             | US10 - Como jogador, quero reconhecer NPCs importantes por seus designs distintivos.                                         | 15                        |
 | TM01             | EP02 - Criação de Personagens | C03 - Criar modelos 2D para NPCs e inimigos                               | F06 - Criar os sprites para os NPCs                                             | US11 - Como narrador, quero que NPCs tenham expressões faciais variadas para enriquecer diálogos.                            | 15                        |
 | TM01             | EP03 - Design de Itens        | C05 - Criar visuais distintos para cada item                              | F08 - Designar ícones únicos para cada tipo de carta e dado                     | US14 - Como jogador, quero identificar rapidamente tipos de cartas/dados por seus ícones durante o combate.                  | 15                        |
 | TM01             | EP03 - Design de Itens        | C05 - Criar visuais distintos para cada item                              | F08 - Designar ícones únicos para cada tipo de carta e dado                     | US15 - Como artista, quero criar ícones que sigam uma sinalização consistente por raridade.                                  | 15                        |
 | TM01             | EP03 - Design de Itens        | C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F11 - Implementar sistema de arrastar e soltar cartas no menu de deck           | US20 - Como jogador, quero reorganizar meu deck arrastando cartas com o mouse/controle.                                      | 15                        |
 | TM01             | EP03 - Design de Itens        | C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F11 - Implementar sistema de arrastar e soltar cartas no menu de deck           | US21 - Como UX designer, quero fornecer feedback visual durante a interação de arrastar (hover, drop válido/inválido).       | 15                        |
 | TM01             | EP03 - Design de Itens        | C29 - Integrar o sistema de artefatos                                     | F48 - Criar o menu de artefatos                                                 | US94 - Como jogador, quero visualizar minha coleção de artefatos.                                                            | 15                        |
 | TM01             | EP03 - Design de Itens        | C29 - Integrar o sistema de artefatos                                     | F48 - Criar o menu de artefatos                                                 | US95 - Como designer, quero que o menu de artefatos mostre progresso de conquistas relacionadas.                             | 15                        |
 | TM01             | EP03 - Design de Itens        | C29 - Integrar o sistema de artefatos                                     | F49 - Desbloquear os artefatos como colecionáveis                               | US96 - Como jogador, quero receber artefatos como recompensa por desafios significativos.                                    | 15                        |
 | TM01             | EP03 - Design de Itens        | C29 - Integrar o sistema de artefatos                                     | F49 - Desbloquear os artefatos como colecionáveis                               | US97 - Como desenvolvedor, quero rastrear artefatos desbloqueados via sistema de save.                                       | 15                        |
 | TM02             | EP04 - Combate                | C08 - Implementar o sistema das cartas                                    | F15 - Aplicar efeitos específicos das cartas no inimigo ou jogador              | US28 - Como jogador, quero ver feedback visual claro quando efeitos de cartas são ativados (positivos/negativos).            | 15                        |
 | TM02             | EP05 - Eventos Aleatórios     | C09 - Gerar eventos com consequências variadas                            | F16 - Criar tabela de eventos com tipos: positivos, negativos e neutros         | US31 - Como jogador, quero encontrar eventos aleatórios para me beneficiar (ou não) em jogo.                                 | 15                        |
 | TM02             | EP07 - Loja                   | C14 - Programar sistema de moedas e economia                              | F26 - Implementar sistema de moeda obtida em batalhas ou eventos                | US50 - Como jogador, quero ganhar moedas de forma proporcional ao desafio superado.                                          | 15                        |
 | TM03             | EP08 - Menus de Navegação     | C16 - Implementar transições visuais entre menus                          | F30 - Adicionar transições animadas entre menus                                 | US58 - Como jogador, quero transições suaves entre menus que não causem desorientação.                                       | 15                        |
 | TM03             | EP08 - Menus de Navegação     | C16 - Implementar transições visuais entre menus                          | F30 - Adicionar transições animadas entre menus                                 | US59 - Como desenvolvedor, quero otimizar animações para que não aumentem significativamente o tempo de carregamento.        | 15                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C17 - Mostrar informações de combate e status do jogador                  | F32 - Exibir status do jogador (vida, cartas, dados) durante o combate          | US63 - Como UX designer, quero organizar as informações prioritárias no HUD de forma hierárquica.                            | 15                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C18 - Exibir efeitos visuais em ações como dano ou combo                  | F34 - Criar efeitos visuais de danos e combos                                   | US67 - Como artista, quero diferenciar visualmente tipos de dano (inimigo, jogador)                                          | 15                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C18 - Exibir efeitos visuais em ações como dano ou combo                  | F35 - Criar efeitos visuais de interação com objetos                            | US68 - Como jogador, quero perceber claramente quando um objeto no cenário é interagível.                                    | 15                        |
 | TM04             | EP10 - Composição de Músicas  | C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F36 - Compor trilhas sonoras únicas para cada círculo com base em ambientação   | US70 - Como jogador, quero músicas que reforcem a identidade única de cada círculo do Inferno.                               | 15                        |
 | TM04             | EP10 - Composição de Músicas  | C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F37 - Mixar músicas em camadas (base, combate, tensão) para cada cenário        | US72 - Como jogador, quero transições dinâmicas entre estados musicais (mapa -> combate).                                    | 15                        |
 | TM04             | EP10 - Composição de Músicas  | C20 - Implementar variações dinâmicas na música conforme ações do jogador | F38 - Mudar a intensidade da trilha com base na ação do jogador (ex: combate)   | US74 - Como jogador, quero que a música reflita a tensão do momento (ex: chefes finais tenham trilhas épicas).               | 15                        |
 | TM04             | EP10 - Composição de Músicas  | C20 - Implementar variações dinâmicas na música conforme ações do jogador | F38 - Mudar a intensidade da trilha com base na ação do jogador (ex: combate)   | US75 - Como designer de áudio, quero implementar parâmetros dinâmicos que modifiquem a música com base no estado do jogo.    | 15                        |
 | TM04             | EP10 - Composição de Músicas  | C20 - Implementar variações dinâmicas na música conforme ações do jogador | F39 - Adicionar transições suaves entre trilhas com base em gatilhos do jogo    | US76 - Como jogador, quero transições musicais suaves ao mudar de área ou entrar em combate.                                 | 15                        |
 | TM04             | EP11 - Efeitos Sonoros        | C21 - Adicionar sons para interações, menus e ações de combate            | F40 - Criar sons para interações e menus                                        | US78 - Como jogador, quero feedback auditivo único para ações importantes.                                                   | 15                        |
 | TM04             | EP11 - Efeitos Sonoros        | C21 - Adicionar sons para interações, menus e ações de combate            | F41 - Adicionar sons únicos para usos de carta e efeitos de combo               | US80 - Como jogador, quero sons distintos para cartas de diferentes raridades.                                               | 15                        |
 | TM04             | EP11 - Efeitos Sonoros        | C21 - Adicionar sons para interações, menus e ações de combate            | F41 - Adicionar sons únicos para usos de carta e efeitos de combo               | US81 - Como desenvolvedor, quero que sons de cartas sejam espacializados quando aplicável.                                   | 15                        |
 | TM04             | EP11 - Efeitos Sonoros        | C22 - Integrar efeitos sonoros com sistema de animação                    | F42 - Integrar sons com animações de ataque e interação                         | US82 - Como jogador, quero sincronia perfeita entre sons e animações de ataques.                                             | 15                        |
 | TM04             | EP11 - Efeitos Sonoros        | C22 - Integrar efeitos sonoros com sistema de animação                    | F43 - Integrar sons dos NPCs                                                    | US85 - Como desenvolvedor, quero que diálogos importantes tenham prioridade sonora sobre ambientes.                          | 15                        |
 | TM05             | EP12 - Diálogos               | C27 - Escrever os diálogos do jogo                                        | F44 - Escrever diálogos ramificados para personagens importantes                | US86 - Como jogador, quero que minhas escolhas nos diálogos impactem a narrativa e o mundo.                                  | 15                        |
 | TM05             | EP12 - Diálogos               | C27 - Escrever os diálogos do jogo                                        | F44 - Escrever diálogos ramificados para personagens importantes                | US87 - Como escritor, quero estruturar diálogos em árvores lógicas que sejam fáceis de implementar.                          | 15                        |
 | TM02             | EP06 - Sistema de Trilha      | C11 - Gerar caminhos de progressão aleatórios entre níveis                | F20 - Gerar caminhos aleatórios conectando cenários com regras de progressão    | US38 - Como jogador, quero utilizar um sistema de navegação em trilha aleatório                                              | 12.5                      |
 | TM03             | EP08 - Menus de Navegação     | C16 - Implementar transições visuais entre menus                          | F31 - Implementar sons de menu sincronizados com animações                      | US61 - Como designer de som, quero criar uma identidade auditiva consistente para todas as interfaces.                       | 12.5                      |
 | TM01             | EP02 - Criação de Personagens | C04 - Integrar personagens com sistema de combate                         | F07 - Integrar eventos de animação com sistema de combate                       | US12 - Como jogador, quero ver animações fluidas durante ataques e defesas no combate.                                       | 10                        |
 | TM01             | EP03 - Design de Itens        | C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F10 - Exibir dados coletados e regras do jogo no menu do "saco de dados"        | US18 - Como jogador, quero consultar regras e estatísticas dos meus dados a qualquer momento.                                | 10                        |
 | TM01             | EP03 - Design de Itens        | C06 - Integrar itens com sistema de menu (saco de dados e deck)           | F10 - Exibir dados coletados e regras do jogo no menu do "saco de dados"        | US19 - Como desenvolvedor, quero organizar as informações do saco de dados em categorias intuitivas.                         | 10                        |
 | TM02             | EP04 - Combate                | C07 - Implementar sistema de lançamento de dados                          | F13 - Pegar o valor atual do dado no 3D e exibir resultado em HUD               | US25 - Como desenvolvedor, quero formatar a exibição do resultado para ser legível em diferentes resoluções.                 | 10                        |
 | TM02             | EP04 - Combate                | C08 - Implementar o sistema das cartas                                    | F14 - Implementar sistema de combos a partir das cartas                         | US27 - Como game designer, quero criar um sistema de combos para dados.                                                      | 10                        |
 | TM02             | EP06 - Sistema de Trilha      | C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F22 - Criar mapa da trilha com visualização dos caminhos possíveis              | US42 - Como jogador, quero visualizar meu progresso e opções futuras no mapa de forma intuitiva.                             | 10                        |
 | TM02             | EP06 - Sistema de Trilha      | C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F22 - Criar mapa da trilha com visualização dos caminhos possíveis              | US43 - Como UX designer, quero representar visualmente os tipos de encontros possíveis em cada nó do mapa.                   | 10                        |
 | TM02             | EP07 - Loja                   | C13 - Implementar interface de compra de cartas                           | F24 - Exibir loja com seções de cartas disponíveis, raridade e custo            | US46 - Como jogador, quero visualizar estatísticas e custos das cartas antes de comprar.                                     | 10                        |
 | TM02             | EP07 - Loja                   | C13 - Implementar interface de compra de cartas                           | F24 - Exibir loja com seções de cartas disponíveis, raridade e custo            | US47 - Como desenvolvedor, quero realizar uma tabela de possibilidades para aquisição das cartas                             | 10                        |
 | TM02             | EP07 - Loja                   | C14 - Programar sistema de moedas e economia                              | F27 - Exibir saldo do jogador na interface da loja                              | US53 - Como desenvolvedor, quero formatar a exibição de moedas para ser legível mesmo em valores altos.                      | 10                        |
 | TM03             | EP08 - Menus de Navegação     | C15 - Criar estrutura de menus                                            | F28 - Criar menus para: Jogo, Loja, Deck, Dados, Pausa, Configurações, Créditos | US54 - Como jogador, quero acessar todas as funcionalidades principais em no máximo 3 cliques a partir do menu inicial.      | 10                        |
 | TM03             | EP08 - Menus de Navegação     | C15 - Criar estrutura de menus                                            | F28 - Criar menus para: Jogo, Loja, Deck, Dados, Pausa, Configurações, Créditos | US55 - Como desenvolvedor, quero implementar um sistema de navegação por teclado/controle seguindo padrões acessíveis.       | 10                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C17 - Mostrar informações de combate e status do jogador                  | F32 - Exibir status do jogador (vida, cartas, dados) durante o combate          | US62 - Como jogador, quero monitorar minha vida, recursos e status atual durante o combate sem obstruir a visão.             | 10                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C17 - Mostrar informações de combate e status do jogador                  | F33 - Exibir informações do inimigo                                             | US64 - Como jogador, quero ver a vida e status dos inimigos para planejar minha estratégia.                                  | 10                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C17 - Mostrar informações de combate e status do jogador                  | F33 - Exibir informações do inimigo                                             | US65 - Como desenvolvedor, quero implementar um sistema de barras de vida que escalone para diferentes tamanhos de inimigos. | 10                        |
 | TM03             | EP09 - HUD e Feedback Visual  | C18 - Exibir efeitos visuais em ações como dano ou combo                  | F34 - Criar efeitos visuais de danos e combos                                   | US66 - Como jogador, quero feedback visual imediato quando causo ou recebo dano.                                             | 10                        |
 | TM04             | EP10 - Composição de Músicas  | C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F36 - Compor trilhas sonoras únicas para cada círculo com base em ambientação   | US71 - Como compositor, quero criar leitmotivs que evoluam conforme o jogador progride.                                      | 10                        |
 | TM04             | EP10 - Composição de Músicas  | C19 - Criar trilhas sonoras adaptadas a cada círculo do Inferno           | F37 - Mixar músicas em camadas (base, combate, tensão) para cada cenário        | US73 - Como desenvolvedor, quero um sistema que alterne entre camadas musicais sem cortes ou repetições bruscas.             | 10                        |
 | TM05             | EP12 - Diálogos               | C27 - Escrever os diálogos do jogo                                        | F45 - Organizar sistema de diálogo em planilha                                  | US89 - Como tradutor, quero acesso estruturado a todos os textos do jogo para tradução.                                      | 10                        |
 | TM05             | EP12 - Diálogos               | C28 - Implementar sistema de taunt de elites e boss para o jogador        | F46 - Criar falas provocativas para elites e chefes com base no combate         | US90 - Como jogador, quero que chefes reajam às minhas ações durante o combate com falas imersivas.                          | 10                        |
 | TM05             | EP12 - Diálogos               | C28 - Implementar sistema de taunt de elites e boss para o jogador        | F46 - Criar falas provocativas para elites e chefes com base no combate         | US91 - Como escritor, quero criar taunts que variem conforme a progressão do jogador no combate.                             | 10                        |
 | TM02             | EP04 - Combate                | C08 - Implementar o sistema das cartas                                    | F14 - Implementar sistema de combos a partir das cartas                         | US26 - Como jogador, quero executar combos específicos ao jogar sequências de cartas para efeitos.                           | 7.5                       |
 | TM02             | EP05 - Eventos Aleatórios     | C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F19 - Integrar eventos aleatórios como interrupções no fluxo principal          | US36 - Como jogador, quero que eventos aleatórios ofereçam pausas estratégicas no fluxo principal.                           | 7.5                       |
 | TM02             | EP05 - Eventos Aleatórios     | C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F19 - Integrar eventos aleatórios como interrupções no fluxo principal          | US37 - Como desenvolvedor, quero implementar um sistema que garanta que eventos não travem o progresso principal.            | 7.5                       |
 | TM02             | EP05 - Eventos Aleatórios     | C09 - Gerar eventos com consequências variadas                            | F16 - Criar tabela de eventos com tipos: positivos, negativos e neutros         | US30 - Como game designer, quero criar eventos com probabilidades balanceadas para evitar repetição excessiva.               | 6.67                      |
 | TM02             | EP05 - Eventos Aleatórios     | C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F18 - Definir pontos de ativação para eventos aleatórios no mapa                | US34 - Como designer, quero distribuir eventos aleatórios de forma a manter um ritmo de jogo equilibrado.                    | 6.67                      |
 | TM04             | EP11 - Efeitos Sonoros        | C22 - Integrar efeitos sonoros com sistema de animação                    | F42 - Integrar sons com animações de ataque e interação                         | US83 - Como animador, quero marcas temporais precisas para sincronizar efeitos sonoros.                                      | 6                         |
 | TM01             | EP03 - Design de Itens        | C05 - Criar visuais distintos para cada item                              | F09 - Criar animações de aquisição e uso visual de cada item                    | US16 - Como jogador, quero ver feedback visual ao adquirir novos itens.                                                      | 5                         |
 | TM01             | EP03 - Design de Itens        | C05 - Criar visuais distintos para cada item                              | F09 - Criar animações de aquisição e uso visual de cada item                    | US17 - Como desenvolvedor, quero que animações de itens não interrompam o fluxo do jogo.                                     | 5                         |
 | TM02             | EP04 - Combate                | C07 - Implementar sistema de lançamento de dados                          | F12 - Criar sistema de lançamento de dados com animação visual                  | US22 - Como jogador, quero lançar dados com física realista e resultados claramente visíveis.                                | 5                         |
 | TM02             | EP04 - Combate                | C07 - Implementar sistema de lançamento de dados                          | F12 - Criar sistema de lançamento de dados com animação visual                  | US23 - Como desenvolvedor, quero calcular resultados com base na posição final do dado 3D.                                   | 5                         |
 | TM02             | EP04 - Combate                | C07 - Implementar sistema de lançamento de dados                          | F13 - Pegar o valor atual do dado no 3D e exibir resultado em HUD               | US24 - Como jogador, quero ver imediatamente o valor do dado em uma interface clara durante o combate.                       | 5                         |
 | TM02             | EP05 - Eventos Aleatórios     | C09 - Gerar eventos com consequências variadas                            | F17 - Escrever descrições e consequências únicas para cada evento               | US32 - Como narrador, quero que eventos tenham textos imersivos que complementem o tom do jogo.                              | 5                         |
 | TM02             | EP05 - Eventos Aleatórios     | C09 - Gerar eventos com consequências variadas                            | F17 - Escrever descrições e consequências únicas para cada evento               | US33 - Como jogador, quero entender claramente as consequências de minhas escolhas nos eventos.                              | 5                         |
 | TM02             | EP05 - Eventos Aleatórios     | C10 - Integrar eventos aleatórios ao fluxo de gameplay                    | F18 - Definir pontos de ativação para eventos aleatórios no mapa                | US35 - Como jogador, quero poder selecionar o evento aleatório na trilha.                                                    | 5                         |
 | TM02             | EP06 - Sistema de Trilha      | C11 - Gerar caminhos de progressão aleatórios entre níveis                | F20 - Gerar caminhos aleatórios conectando cenários com regras de progressão    | US39 - Como desenvolvedor, quero garantir que caminhos sejam gerados aleatóriamente.                                         | 5                         |
 | TM02             | EP06 - Sistema de Trilha      | C11 - Gerar caminhos de progressão aleatórios entre níveis                | F21 - Definir pesos e condições para gerar as bifurcações                       | US40 - Como game designer, quero controlar a probabilidade de certos tipos de encontros aparecerem em cada nível.            | 5                         |
 | TM02             | EP06 - Sistema de Trilha      | C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F23 - Permitir seleção de caminho com botão de confirmação                      | US44 - Como jogador, quero confirmar minha escolha de caminho antes de prosseguir para evitar erros.                         | 5                         |
 | TM02             | EP06 - Sistema de Trilha      | C12 - Exibir mapa da trilha com opções de escolha visíveis ao jogador     | F23 - Permitir seleção de caminho com botão de confirmação                      | US45 - Como desenvolvedor, quero implementar um fluxo para ser seguido pelo jogador                                          | 5                         |
 | TM02             | EP07 - Loja                   | C13 - Implementar interface de compra de cartas                           | F25 - Criar pop-up de confirmação de compra com descrição da carta              | US48 - Como jogador, quero ver detalhes completos da carta antes de confirmar a compra.                                      | 5                         |
 | TM02             | EP07 - Loja                   | C13 - Implementar interface de compra de cartas                           | F25 - Criar pop-up de confirmação de compra com descrição da carta              | US49 - Como UX designer, quero evitar compras acidentais com confirmação clara mas não intrusiva.                            | 5                         |
 | TM02             | EP07 - Loja                   | C14 - Programar sistema de moedas e economia                              | F27 - Exibir saldo do jogador na interface da loja                              | US52 - Como jogador, quero ver meu saldo atualizado em tempo real durante compras.                                           | 5                         |
 | TM05             | EP12 - Diálogos               | C27 - Escrever os diálogos do jogo                                        | F45 - Organizar sistema de diálogo em planilha                                  | US88 - Como desenvolvedor, quero exportar diálogos para o engine a partir de planilhas.                                      | 5                         |
 | TM05             | EP12 - Diálogos               | C28 - Implementar sistema de taunt de elites e boss para o jogador        | F47 - Integrar sistema de taunts com entrada de combate do jogador              | US93 - Como desenvolvedor, quero implementar um sistema de triggers que não interrompa o fluxo do combate.                   | 5                         |
 | TM01             | EP02 - Criação de Personagens | C04 - Integrar personagens com sistema de combate                         | F07 - Integrar eventos de animação com sistema de combate                       | US13 - Como desenvolvedor, quero sincronizar eventos de animação com triggers do sistema de combate.                         | 3.33                      |
 | TM02             | EP06 - Sistema de Trilha      | C11 - Gerar caminhos de progressão aleatórios entre níveis                | F21 - Definir pesos e condições para gerar as bifurcações                       | US41 - Como jogador, quero sentir um senso de escolha e análise a partir das bifurcações.                                    | 3                         |
 | TM04             | EP10 - Composição de Músicas  | C20 - Implementar variações dinâmicas na música conforme ações do jogador | F39 - Adicionar transições suaves entre trilhas com base em gatilhos do jogo    | US77 - Como desenvolvedor, quero garantir que transições musicais não causem stuttering ou lag.                              | 3                         |
 | TM01             | EP01 - Criação de Cenários    | C02 - Otimizar performance visual dos cenários                            | F03 - Definir aspectos técnicos referentes à performance                        | US05 - Como desenvolvedor, quero otimizar polígonos e texturas para manter uma taxa estável de FPS                           | 1                         |
 | TM01             | EP01 - Criação de Cenários    | C02 - Otimizar performance visual dos cenários                            | F03 - Definir aspectos técnicos referentes à performance                        | US06 - Como jogador, quero uma experiência fluida sem travamentos durante transições de cenário.                             | 1                         |
 | TM01             | EP01 - Criação de Cenários    | C02 - Otimizar performance visual dos cenários                            | F04 - Usar instâncias reutilizáveis para objetos do cenário                     | US07 - Como desenvolvedor, quero reutilizar assets de cenário com variações para reduzir carga de memória.                   | 1                         |

## Histórico de Revisões
| Data       | Autor                                      | Alterações                                         |
| ---------- | ------------------------------------------ | -------------------------------------------------- |
| 2025-05-13 | [Mateus Vieira](https://github.com/matix0) | Reestruturação do backlog para maior consistência. |
| 2025-05-14 | [Mateus Vieira](https://github.com/matix0) | Criação do modelo SAFe sem o backlog final         |
| 2025-05-14 | [Mateus Vieira](https://github.com/matix0) | Backlog finalizado e priorizado                    |
