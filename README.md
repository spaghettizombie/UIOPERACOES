# Manual Operacional — Plataforma Táctica GIOE / ISEOP

Documento destinado a operadores e analistas. Estabelece as funcionalidades disponíveis, os procedimentos de utilização e os fluxos operacionais recomendados para a plataforma de planeamento e execução táctica.

---

## Índice

1. [Inicialização e Selecção de Perfil](#1-inicialização-e-selecção-de-perfil)
2. [Navegação Cartográfica](#2-navegação-cartográfica)
3. [Sistema de Pontos Tácticos](#3-sistema-de-pontos-tácticos)
4. [Instrumentos de Medição](#4-instrumentos-de-medição)
5. [Caixas de Comentário](#5-caixas-de-comentário)
6. [Linha de Visão (LOS)](#6-linha-de-visão-los)
7. [Geolocalização (GPS)](#7-geolocalização-gps)
8. [Cálculo de Itinerários (ORS)](#8-cálculo-de-itinerários-ors)
9. [Análise Solar e Lunar](#9-análise-solar-e-lunar)
10. [Análise por Inteligência Artificial](#10-análise-por-inteligência-artificial)
11. [Operação em Modo Offline](#11-operação-em-modo-offline)
12. [Timeline Operacional](#12-timeline-operacional)
13. [Camadas Operacionais](#13-camadas-operacionais)
14. [Análise Meteorológica](#14-análise-meteorológica)
15. [Modo Briefing](#15-modo-briefing)
16. [Permuta de Dados (KMZ/KML)](#16-permuta-de-dados-kmzkml)
17. [Geração de Relatórios](#17-geração-de-relatórios)
18. [Captura de Imagem do Mapa](#18-captura-de-imagem-do-mapa)
19. [Histórico e Reversão de Acções](#19-histórico-e-reversão-de-acções)
20. [Atalhos de Teclado](#20-atalhos-de-teclado)
21. [Operação em Dispositivos Móveis](#21-operação-em-dispositivos-móveis)
22. [Configuração Visual](#22-configuração-visual)
23. [Procedimento Operacional Recomendado](#23-procedimento-operacional-recomendado)
24. [Resolução de Anomalias](#24-resolução-de-anomalias)

---

## 1. Inicialização e Selecção de Perfil

A plataforma exige a selecção de um perfil operacional no arranque inicial:

- **GIOE** — Grupo de Intervenção de Operações Especiais. Identidade cromática vermelha.
- **ISEOP** — Intervenção em Situações Especiais de Ordem Pública. Identidade cromática verde.

A selecção determina:

- A cor primária aplicada a barreiras, perímetros e elementos de sinalização;
- O cabeçalho de identificação dos relatórios em formato PDF e Word;
- O prefixo dos ficheiros exportados.

A escolha é persistida em sessão e pode ser alterada em qualquer momento através do indicador no canto inferior direito da barra de estado. A alteração de perfil não compromete os dados operacionais já registados.

---

## 2. Navegação Cartográfica

### 2.1 Controlos básicos

| Acção | Procedimento |
|---|---|
| Deslocar mapa | Arrastar com botão esquerdo do rato |
| Aproximar/afastar | Roda do rato ou controlos `+`/`−` |
| Zoom dirigido | Duplo-clique no ponto de interesse |

### 2.2 Camadas cartográficas disponíveis

A plataforma disponibiliza treze fontes cartográficas, organizadas em quatro grupos:

**Google Maps:** Satélite, Híbrido, Terreno, Ruas

**ESRI:** World Imagery (alta resolução), Topográfico, Streets

**Bing Maps:** Aéreo

**Fontes abertas:** OpenStreetMap, OpenTopoMap, CartoDB Dark, CartoDB Positron, OSM France

### 2.3 Recomendações de utilização

| Cenário operacional | Camada recomendada |
|---|---|
| Análise visual e identificação de objectos | Satélite (Google) ou World Imagery (ESRI) |
| Planeamento em terreno acidentado | OpenTopoMap |
| Operação nocturna / leitura em condições de baixa luminosidade | CartoDB Dark |
| Análise de edificado urbano | OSM France ou Híbrido |

### 2.4 Indicadores cartográficos

Uma escala métrica é mantida no canto inferior esquerdo, ajustando-se automaticamente ao nível de zoom para apoiar estimativas dimensionais imediatas.

---

## 3. Sistema de Pontos Tácticos

A plataforma disponibiliza vinte e nove tipos de marcadores agrupados por função operacional.

### 3.1 Métodos de criação

- **Toolbar:** activar a ferramenta de marcação e seleccionar a posição no mapa.
- **Menu contextual:** botão direito sobre a posição desejada → "Fixar ponto aqui".

### 3.2 Categorias e tipos

**Navegação e posicionamento**

| Sigla | Designação |
|---|---|
| WPT | Waypoint |
| OP | Posto de Observação |
| BP | Posição de Edifício |
| CP | Checkpoint / Cordão |

**Inteligência sobre adversário**

| Sigla | Designação |
|---|---|
| TGT | Alvo confirmado (HVT) |
| SUS | Suspeito (não confirmado) |
| HOS | Refém |
| VIP | Pessoa protegida |

**Forças Amigas** (ordenadas por hierarquia operacional)

| Sigla | Designação | Identidade visual |
|---|---|---|
| PC | Posto de Comando | Fundo verde escuro · borda e texto dourado |
| GIO | UI — GIOE | Fundo vermelho · borda e texto dourado |
| GIP | UI — GIOP | Fundo preto · borda e texto dourado |
| PAT | GNR — Patrulha | Fundo verde escuro · borda e texto dourado |
| PSP | PSP — Patrulha | Fundo azul escuro · borda e texto branco |
| BV | BV — Bombeiros | Fundo vermelho · borda e texto branco |
| INM | INM — INEM | Fundo azul médio · borda e texto branco |
| K9 | K9 — Cinotécnica | Fundo preto · borda e texto dourado |
| EOD | Engenhos / Desactivação | Cor padrão |
| SNP | Sniper / Overwatch | Cor padrão |
| STK | Stack (pré-entrada) | Cor padrão |
| BRE | Breach point | Cor padrão |
| NEG | Negociador | Cor padrão |
| DRN | Drone / UAV | Cor padrão |
| FRP | Força amiga (genérica) | Cor padrão |

A diferenciação cromática entre forças com identidade gráfica institucional (PC, GIO, GIP, PAT, K9, PSP, BV, INM) e meios especiais permite identificação imediata em vista táctica.

**Manobra e objectivos**

| Sigla | Designação |
|---|---|
| OBJ | Objectivo da operação |
| INF | Ponto de infiltração |
| EXF | Ponto de exfiltração |

**Sustentação**

| Sigla | Designação |
|---|---|
| CCP | Casualty Collection Point (MEDEVAC) |
| SUP | Reabastecimento |
| COM | Posto de comunicações |
| HLZ | Heliport / Helicopter Landing Zone |

**Mobilidade**

| Sigla | Designação |
|---|---|
| VEH | Viatura amiga |
| TVE | Viatura-alvo |

**Risco**

| Sigla | Designação |
|---|---|
| HZD | Hazard / Perigo |

### 3.3 Atributos por marcador

Cada marcador suporta os seguintes atributos editáveis:

| Atributo | Valores |
|---|---|
| Nome | Texto livre |
| Descrição | Texto livre |
| Notas | Texto livre |
| Prioridade | Alta, Média, Baixa |
| Estado | Planeado, Activo, Comprometido, Neutralizado |
| Confiança | Alta, Média, Baixa |

Os atributos são reflectidos visualmente no marcador:
- Prioridade alta apresenta indicador pulsante a vermelho;
- Estado "Comprometido" apresenta sobreposição cruciforme vermelha;
- Estado "Neutralizado" apresenta opacidade reduzida;
- Confiança média ou baixa apresenta marca interrogativa em amarelo ou vermelho.

### 3.4 Acções sobre marcadores

A selecção de um marcador apresenta um popup com:

- Coordenadas em formato decimal e UTM
- Altitude (obtida automaticamente)
- Atributos configurados
- Acções disponíveis: cálculo de itinerário desde a posição GPS, edição, centragem, remoção

O menu contextual (botão direito) apresenta adicionalmente:

- Cálculo de itinerário desde a posição actual
- Abertura no Google Maps

A reposicionação é feita por arrastamento.

---

## 4. Instrumentos de Medição

A barra de ferramentas integra onze instrumentos de medição. Cada selecção apresenta na barra inferior um indicativo do procedimento esperado.

### 4.1 Distância linear
Sequência de cliques para definir os vértices, finalizando com duplo-clique ou tecla Enter. Apresenta a distância total e por segmento.

### 4.2 Área poligonal
Definição dos vértices com cliques sucessivos. Duplo-clique fecha o polígono. O resultado é apresentado em metros quadrados ou quilómetros quadrados, conforme magnitude.

### 4.3 Raio circular
Dois cliques: centro e ponto de raio. Apresenta o raio em metros.

### 4.4 Azimute geodésico
Dois cliques: origem e destino. Apresenta ângulo (0–360°) e distância.

### 4.5 Anéis de alcance
Um clique no centro gera automaticamente três círculos concêntricos a 500 m, 1 km e 2 km, indicados para visualização de perímetros de protecção ou cobertura.

### 4.6 Sector de tiro
Dois cliques: posição de tiro e ponto-objectivo. Desenha um cone de 60° na direcção definida.

### 4.7 Itinerário multi-segmento
Sequência de waypoints com duplo-clique para finalizar. Apresenta distância acumulada.

### 4.8 Zona de exclusão
Dois cliques: centro e raio. Visualização distinta com tracejado vermelho.

### 4.9 Barreira / Corte de estrada
Dois cliques nas extremidades da barreira. Gera um rectângulo escuro perpendicular ao vector definido, com etiqueta de comprimento.

### 4.10 Quadrícula militar (MGRS)
Sobreposição de grelha conforme padrão militar. Activável também através da tecla `Q`.

### 4.11 Limpeza
Acção de limpeza global de medições, reversível por meio do histórico (Ctrl+Z).

---

## 5. Caixas de Comentário

Marcadores textuais permanentemente visíveis no mapa, em formato de balão, destinados a anotações operacionais contextuais.

### 5.1 Características

- Limite de oitenta caracteres por anotação;
- Três esquemas cromáticos disponíveis:
  - Branco (fundo branco, texto preto, contorno preto)
  - Preto (fundo preto, texto branco, contorno branco)
  - Vermelho (fundo vermelho, texto branco, contorno branco)
- Forma vectorial única com extremidade descendente integrada com a aresta esquerda do balão.

### 5.2 Procedimento

1. Activação do instrumento na barra de ferramentas;
2. Selecção da posição no mapa;
3. Introdução do texto e selecção do esquema cromático;
4. Confirmação.

### 5.3 Manutenção

- A selecção do balão reabre o painel de edição;
- A reposicionação é feita por arrastamento;
- A remoção é executada através do menu contextual ou eliminando o conteúdo textual no painel de edição.

### 5.4 Aplicações típicas

- Identificação de zonas de reunião
- Sinalização de obstáculos contextuais
- Marcação de meios de vigilância
- Indicação de instruções temporais relativas

As anotações são integradas nas capturas de imagem e nos relatórios gerados.

---

## 6. Linha de Visão (LOS)

Ferramenta de análise topográfica para determinação de visibilidade entre dois pontos, considerando o relevo do terreno.

### 6.1 Procedimento

1. Activação do instrumento na barra de ferramentas;
2. Primeiro clique: posição do observador;
3. Segundo clique: posição do alvo;
4. Aguardar consulta automática do perfil de elevação.

### 6.2 Metodologia

A plataforma amostra trinta e dois pontos ao longo do segmento e consulta o serviço Open-Elevation para obtenção das altitudes correspondentes. É considerada uma altura adicional de 1,7 metros para o observador e para o alvo. Para cada ponto intermédio, a altura da linha directa entre observador e alvo é comparada com a altitude do terreno.

### 6.3 Apresentação de resultados

**Sem obstrução:** linha contínua a verde, com indicação da distância total e da folga mínima sobre o terreno.

**Com obstrução:** linha tracejada a vermelho, marcação do primeiro ponto de obstrução e indicação da distância a que ocorre.

O resultado é registado como medição persistente, sendo incluído nas exportações e relatórios.

---

## 7. Geolocalização (GPS)

Dois controlos no canto superior direito do mapa permitem o uso de geolocalização.

### 7.1 Modos de operação

**Toque curto** no controlo principal: fixação única da posição com indicador pulsante e círculo de precisão.

**Toque prolongado** (aproximadamente um segundo): activação do modo de seguimento contínuo, com registo do trajecto.

**Marcação de posição:** controlo dedicado para criação imediata de waypoint na posição actual, designado automaticamente como `GPS-HHMM`.

### 7.2 Indicadores

- Marcador azul pulsante na posição actual;
- Círculo correspondente à precisão fornecida pelo dispositivo;
- Tooltip com altitude, velocidade (km/h) e direcção;
- Na barra de estado, com pontos no mapa, é apresentado o ponto táctico mais próximo, distância e azimute.

### 7.3 Considerações operacionais

- A precisão típica em dispositivos móveis com vista ao céu é de 5 a 15 metros;
- Em estações fixas sem GPS dedicado, a precisão pode degradar-se para escalas de centenas de metros, por dependência de triangulação Wi-Fi ou IP;
- O acesso à geolocalização requer autorização do utilizador, solicitada pelo navegador no primeiro uso;
- A interrupção de visibilidade da aplicação suspende o seguimento, sendo retomado automaticamente sem nova autorização.

---

## 8. Cálculo de Itinerários (ORS)

Integração com o serviço OpenRouteService para cálculo de itinerários por rede viária.

### 8.1 Configuração

A utilização requer uma chave de acesso, obtida gratuitamente em `openrouteservice.org/dev`. O limite gratuito é de mil pedidos por dia.

A configuração da chave é feita através do menu contextual (botão direito) sobre o controlo de itinerários na barra de ferramentas.

### 8.2 Procedimentos de cálculo

**Itinerário entre dois pontos arbitrários:**
1. Activação do instrumento;
2. Selecção do ponto de origem;
3. Selecção do ponto de destino.

**Itinerário desde a posição actual até um marcador:**
1. Activação do GPS;
2. Selecção do marcador de destino;
3. Activação da opção "Rota Daqui" no popup.

### 8.3 Apresentação

O itinerário é representado por uma linha a verde fluorescente, com marcadores nas extremidades e etiqueta central indicando distância em quilómetros e tempo estimado em minutos. A vista é automaticamente ajustada para visualização integral.

### 8.4 Permuta de chaves

A chave de acesso pode ser exportada em formato JSON e importada em estações distintas, facilitando a configuração coordenada de equipas.

### 8.5 Códigos de erro

| Mensagem | Causa | Acção |
|---|---|---|
| Sem ligação à API | Indisponibilidade de rede | Verificar conectividade |
| Chave inválida ou bloqueada | Credencial inactiva | Reverificar em openrouteservice.org |
| Limite diário excedido | Mil pedidos atingidos | Aguardar reposição diária |
| Não encontrou rota | Pontos sem rede viária acessível | Reposicionar pontos |

---

## 9. Análise Solar e Lunar

Painel de informação astronómica com cálculo de ascensão solar, ocaso, posições orbitais e fases lunares.

### 9.1 Acesso

Controlo dedicado na barra de ferramentas. Atalho: tecla `L`.

### 9.2 Informação solar

- Hora do nascer-do-sol
- Hora do pôr-do-sol
- Hora do zénite (passagem meridiana)
- Azimute solar para o instante de referência
- Elevação solar para o instante de referência
- Duração do dia

### 9.3 Informação lunar

- Hora do nascer da lua
- Hora do pôr da lua
- Fase lunar nominal
- Percentagem de iluminação

### 9.4 Crepúsculos militares

- BMNT (Beginning Morning Nautical Twilight): astronómico (-18°), náutico (-12°), civil (-6°)
- EENT (End Evening Nautical Twilight): civil, náutico, astronómico

### 9.5 Simulação temporal

Interface dedicada à projecção de condições astronómicas em horários específicos:

- Cursor de minutos do dia (resolução de cinco minutos);
- Botões dedicados para fixação imediata em hora actual, nascer-do-sol, pôr-do-sol e zénite;
- Indicação visual distinta entre modo real-time (verde) e modo simulação (âmbar);
- Recálculo dos valores de azimute e elevação em conformidade com o instante seleccionado.

### 9.6 Projecção cartográfica

A activação do modo de projecção apresenta no mapa três vectores radiais a partir do centro da vista:

- Vector tracejado âmbar: azimute do nascer-do-sol;
- Vector tracejado laranja: azimute do pôr-do-sol;
- Vector contínuo amarelo: azimute solar para o instante de referência (real ou simulado).

Em modo simulação, o vector solar é apresentado mesmo quando a elevação é negativa, com cor cinzenta e tracejado, indicando a posição do astro abaixo do horizonte.

As etiquetas dos valores são apresentadas em branco fluorescente para legibilidade uniforme sobre qualquer base cartográfica.

---

## 10. Análise por Inteligência Artificial

Identificação automática de objectos através de processamento de imagem por modelos de visão.

### 10.1 Provedores suportados

- Gemini (Google) — gratuito, recomendado para utilização inicial
- Groq (LLaMA Vision) — gratuito, latência reduzida
- Mistral Pixtral — gratuito
- OpenRouter — meta-provedor com múltiplos modelos
- Claude (Anthropic)

### 10.2 Procedimento

1. Activação do instrumento na barra de ferramentas (atalho `I`);
2. Selecção do provedor e introdução da credencial;
3. Configuração das categorias de objectos a identificar;
4. Execução da análise.

### 10.3 Apresentação de resultados

Os objectos identificados são representados no mapa por caixas delimitadoras coloridas. O painel lateral apresenta a lista de detecções com indicação do nível de confiança. Cada detecção pode ser convertida em ponto táctico formal.

As credenciais são persistidas localmente.

---

## 11. Operação em Modo Offline

A plataforma mantém capacidade operacional plena sem ligação à rede, condicionada à pré-aquisição da cartografia da área de interesse.

### 11.1 Cache automática

Toda a cartografia visualizada é progressivamente acumulada em cache local. A presença ou ausência de ligação é indicada na barra de estado:

- ONLINE — disponibilidade de rede confirmada;
- OFFLINE — sem disponibilidade de rede.

Um contador apresenta o volume de elementos cartográficos em cache.

### 11.2 Aquisição deliberada de área

Para preparação de operações em zonas com cobertura de rede limitada:

1. Activação do instrumento "Download Área";
2. Definição rectangular da zona de interesse no mapa;
3. Configuração dos parâmetros:
   - Níveis de zoom (recomendado: 13–17 para uso urbano, 11–14 para zonas extensas);
   - Selecção das fontes cartográficas (apenas fontes abertas);
4. Confirmação e monitorização do progresso.

A aquisição pode ser interrompida sem perda dos elementos já adquiridos.

### 11.3 Limpeza de cache

Acção dedicada para eliminação total do conteúdo em cache, com confirmação prévia.

### 11.4 Funcionalidades offline

| Funcionalidade | Disponibilidade offline |
|---|---|
| Cartografia em cache | Disponível |
| Pontos tácticos e medições | Disponível |
| Caixas de comentário | Disponível |
| Permuta KMZ/KML | Disponível |
| Geração de relatórios | Disponível |
| Análise IA | Indisponível |
| Itinerários ORS | Indisponível |
| Linha de visão | Indisponível |
| Meteorologia | Indisponível |

---

## 12. Timeline Operacional

Painel para definição cronológica de eventos sincronizados em torno de uma hora de referência (H-hour).

### 12.1 Acesso

Controlo dedicado na barra de ferramentas. Apresenta janela modal com cronograma horizontal e lista editável de eventos.

### 12.2 Estrutura de cada evento

| Campo | Descrição |
|---|---|
| Offset | Minutos relativos a H-hour. Valores negativos indicam momentos anteriores |
| Etiqueta | Designação curta do evento |
| Equipa | Identificação da equipa responsável |
| Ponto ligado | Associação a um marcador táctico do mapa |
| Descrição | Detalhe operacional |

### 12.3 Cronograma horizontal

Visualização gráfica com:

- Marcador vertical vermelho na posição H-hour;
- Pontos coloridos para cada evento (âmbar quando associado a equipa, ciano caso contrário);
- Etiquetas de offset em formato relativo (H-30, H+15, H+1h:30).

### 12.4 Acções sobre eventos

- Centragem da vista no marcador associado;
- Edição directa de qualquer campo;
- Eliminação individual de eventos;
- Reordenação automática por offset.

### 12.5 Persistência

Os eventos são integrados no histórico de gravação automática, suportando reversão e restauro.

---

## 13. Camadas Operacionais

Sistema de gestão de visibilidade e opacidade por categoria semântica, permitindo focar a apresentação em subconjuntos específicos da informação operacional.

### 13.1 Categorias

| Categoria | Conteúdo |
|---|---|
| Inteligência | TGT, SUS, HOS, VIP |
| Forças Amigas | PC, GIO, GIP, PAT, PSP, BV, INM, K9, EOD, SNP, STK, BRE, NEG, DRN, FRP |
| Logística | CCP, SUP, COM, HLZ |
| Manobra | WPT, OP, BP, CP, OBJ, INF, EXF |
| Especial | VEH, TVE, HZD |
| Medições | Todas as medições registadas |
| Comentários | Todas as caixas de comentário |

### 13.2 Controlos por categoria

- Comutador de visibilidade;
- Cursor de opacidade (0% a 100%);
- Indicador da quantidade de elementos na categoria.

### 13.3 Aplicações

- Briefings sequenciais com revelação progressiva de informação;
- Análise focada num subconjunto específico (ex: apenas Forças Amigas);
- Atenuação de elementos não-essenciais para destaque dos relevantes.

---

## 14. Análise Meteorológica

Integração com OpenWeatherMap para obtenção de condições meteorológicas e previsão.

### 14.1 Configuração

Requer chave de acesso, obtida gratuitamente em `openweathermap.org/api`. Limite gratuito: sessenta pedidos por minuto.

### 14.2 Informação apresentada

**Condições actuais:**
- Temperatura
- Sensação térmica
- Vento (velocidade, direcção em graus, ponto cardeal)
- Humidade relativa
- Pressão atmosférica
- Visibilidade
- Nebulosidade
- Precipitação acumulada na última hora

**Previsão:**
- Cinco dias subsequentes
- Temperatura, ícone meteorológico e descrição para cada dia

### 14.3 Aplicações operacionais

A informação meteorológica é determinante para:

- Planeamento de operações com meios aéreos (drones, helicópteros);
- Avaliação de visibilidade para operações de observação;
- Dimensionamento de equipamento térmico das equipas;
- Análise de impacto ambiental sobre dispersão acústica e olfactiva.

---

## 15. Modo Briefing

Configuração de apresentação que oculta a interface administrativa, mantendo apenas a área cartográfica em ecrã completo.

### 15.1 Activação

Controlo dedicado na barra de ferramentas. A activação:

- Oculta a barra superior, painéis laterais e barra de estado;
- Expande a vista cartográfica para a totalidade do ecrã;
- Apresenta um controlo discreto de saída no canto superior direito.

### 15.2 Saída do modo

- Selecção do controlo de saída;
- Tecla `Escape`.

### 15.3 Aplicação típica

Apresentações em sala de operações ou briefings a equipas, mantendo a interactividade de navegação cartográfica.

---

## 16. Permuta de Dados (KMZ/KML)

Suporte aos formatos KMZ e KML para interoperabilidade com sistemas externos.

### 16.1 Compatibilidade

- Google Earth, Google My Maps
- QGIS
- ATAK (Android Tactical Assault Kit)
- JCATS
- Software cartográfico genérico

### 16.2 Conteúdo exportado

- Pontos tácticos com simbologia, atributos e estados
- Medições geométricas
- Caixas de comentário
- Estrutura organizada em pastas por categoria

### 16.3 Persistência local

A totalidade da sessão é gravada automaticamente em armazenamento local. No arranque seguinte, é apresentada a possibilidade de restauro do estado anterior.

---

## 17. Geração de Relatórios

A plataforma produz documentação operacional em formato PDF e Word, com identidade gráfica adaptada ao perfil seleccionado.

### 17.1 Relatório de Missão (PDF)

Documento estruturado em sete secções:

1. Capa com classificação SEGNAC e identificação do perfil
2. Sumário executivo com indicadores quantitativos
3. Captura cartográfica em alta resolução
4. Inventário detalhado de pontos tácticos
5. Inventário de medições
6. Resultados de análise por inteligência artificial (quando aplicável)
7. Bloco de validação e aprovação com três campos de assinatura

### 17.2 Ficha de Alvo (PDF)

Documento focado em alvo específico (tipo TGT), incluindo:

- Identificação completa
- Avaliação de ameaça (Crítica, Alta, Média, Baixa)
- Síntese de inteligência disponível
- ROE (Rules of Engagement)
- Janela operacional
- Bloco de aprovação
- Classificação SEGNAC 1

### 17.3 Versão Word

Equivalente em formato editável (.doc) para revisão prévia à validação. Compatível com Microsoft Word, LibreOffice e Google Docs.

### 17.4 Aplicação da identidade

| Elemento | GIOE | ISEOP |
|---|---|---|
| Cor de cabeçalho | Vermelho | Verde |
| Designação completa | Grupo de Intervenção de Operações Especiais | Intervenção em Situações Especiais de Ordem Pública |
| Prefixo de ficheiro | GIOE_ | ISEOP_ |

---

## 18. Captura de Imagem do Mapa

Geração de imagem em formato PNG com a totalidade do conteúdo cartográfico visível.

### 18.1 Conteúdo capturado

- Cartografia base seleccionada
- Pontos tácticos e respectivos atributos visuais
- Medições e suas etiquetas
- Caixas de comentário
- Quadrícula militar (quando activa)
- Marcador GPS (quando activo)
- Itinerários ORS calculados

### 18.2 Características

- Resolução triplicada relativamente à do ecrã (5760×3240 px num ecrã FullHD)
- Renderização vectorial de texto e linhas
- Qualidade PNG máxima
- Ausência de marcas de água ou sobreposições

### 18.3 Nomenclatura

`PERFIL_MapaCaptura_AAAA-MM-DDTHH-MM-SS.png`

Formato adequado para inclusão em apresentações, briefings e anexos a relatórios.

---

## 19. Histórico e Reversão de Acções

A plataforma mantém um histórico das últimas trinta acções realizadas.

### 19.1 Activação

- Combinação de teclas `Ctrl+Z` (Windows/Linux) ou `Cmd+Z` (macOS);
- Controlo dedicado na barra de ferramentas.

### 19.2 Acções suportadas

- Criação, edição e remoção de pontos
- Registo de medições
- Limpeza de medições
- Criação, edição e remoção de caixas de comentário
- Reposicionamento de marcadores
- Adição, edição e remoção de eventos timeline

Cada acção revertida apresenta notificação identificativa.

---

## 20. Atalhos de Teclado

| Tecla | Acção |
|---|---|
| `Ctrl+Z` / `Cmd+Z` | Reverter última acção |
| `Q` | Comutar quadrícula militar |
| `O` | Activar instrumento de itinerários |
| `L` | Abrir painel astronómico |
| `I` | Abrir análise por IA |
| `TAB` | Comutar painel lateral |
| `Enter` | Finalizar medição em curso |
| `Esc` | Cancelar acção em curso ou sair do modo briefing |

---

## 21. Operação em Dispositivos Móveis

A plataforma adapta-se a dispositivos com diferentes formatos.

### 21.1 Dispositivos móveis (ecrã reduzido)

- Painéis em sobreposição não-intrusiva;
- Controlos dimensionados para interacção táctil (mínimo 40×40 px);
- Barra de estado em formato condensado;
- Acessos rápidos a "Pontos" e "Painel" no rodapé.

### 21.2 Tablets

- Suporte ao modo desktop completo;
- Comutação opcional para modo móvel.

### 21.3 Interacção táctil

| Gesto | Acção equivalente |
|---|---|
| Toque | Selecção (clique esquerdo) |
| Toque prolongado | Menu contextual (clique direito) |
| Pinça | Zoom |
| Arrastamento com dois dedos | Deslocação do mapa |

### 21.4 Geolocalização em mobilidade

Os dispositivos móveis aproveitam o GPS interno, com precisão típica de 5 a 15 metros, sendo recomendados para utilização em terreno.

---

## 22. Configuração Visual

### 22.1 Tema escuro (configuração padrão)

- Paleta neutra em tons de cinzento;
- Texto principal em branco-suave;
- Realces cromáticos diferenciados por função.

### 22.2 Tema claro

- Comutação através do controlo na barra de estado;
- Indicado para utilização em ambientes com forte iluminação.

### 22.3 Cromatismo da barra de ferramentas

| Categoria | Cor | Exemplos |
|---|---|---|
| Ferramentas básicas | Cinzento | Régua, área, círculo, azimute |
| Objectos especiais | Âmbar | Barreira, comentário |
| Análise | Ciano | Linha de visão, timeline, briefing, camadas, meteorologia, sol/lua, IA, descarregamento |
| Itinerários | Verde fluorescente | ORS |
| Exportação | Verde | KMZ, KML, PNG |
| Importação | Azul | KMZ/KML |
| Acções destrutivas | Vermelho | Limpeza |

---

## 23. Procedimento Operacional Recomendado

### 23.1 Fase de planeamento

1. Selecção do perfil operacional;
2. Posicionamento na zona de operação através da camada satélite;
3. Aquisição da área para operação offline (se aplicável);
4. Marcação dos elementos críticos (TGT, OBJ, HZD);
5. Marcação das forças amigas a empenhar (PC, GIO, GIP, PAT, PSP, BV, INM, K9, etc.);
6. Marcação dos elementos de apoio (WPT, CP, INF, EXF);
7. Validação geométrica através das ferramentas de medição;
8. Análise de linha de visão entre pontos críticos;
9. Definição da timeline operacional com sincronização de equipas;
10. Verificação das condições astronómicas e meteorológicas para a janela operacional;
11. Anotação contextual através de caixas de comentário;
12. Geração do relatório de missão.

### 23.2 Fase de execução

1. Activação da geolocalização;
2. Activação do modo de seguimento contínuo;
3. Anotação dinâmica de observações e ajustes;
4. Captura de imagem do estado final.

### 23.3 Fase de partilha e arquivo

1. Exportação em formato KMZ para distribuição inter-equipas;
2. Exportação em formato PDF para arquivo formal;
3. Anexação da captura PNG a apresentações de pós-operação.

---

## 24. Resolução de Anomalias

| Sintoma | Causa provável | Acção |
|---|---|---|
| Área cartográfica em cinza | Sem ligação e fora da cache | Voltar a área em cache ou restabelecer ligação |
| Solicitação repetida de geolocalização | Ausência de HTTPS ou modo anónimo | Aceder via HTTPS e fora de modo anónimo |
| Falha em itinerário ORS | Credencial inválida ou limite atingido | Verificar credencial; aguardar reposição diária |
| Captura PNG sem cartografia | Tiles não totalmente carregados | Aguardar antes de capturar |
| Trabalho perdido após fecho | — | Restauro automático ao reabrir, com confirmação |
| Repor estado inicial | — | Limpeza de cache do navegador para o domínio |

---

*Plataforma desenvolvida por CO/DI/CI — FJCC, para apoiar análise táctica e o planeamento operacional.*
