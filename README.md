# Manual do Utilizador — Plataforma Táctica GIOE / ISEOP

Bem-vindo. Este guia explica como usar todas as funcionalidades da plataforma. Não precisas de conhecimento técnico — basta seguir os passos descritos.

---

## Índice

1. [Primeiros Passos](#1-primeiros-passos)
2. [Navegar no Mapa](#2-navegar-no-mapa)
3. [Marcar Pontos Tácticos](#3-marcar-pontos-tácticos)
4. [Fazer Medições](#4-fazer-medições)
5. [Adicionar Comentários](#5-adicionar-comentários)
6. [Usar o GPS](#6-usar-o-gps)
7. [Calcular Rotas por Estrada](#7-calcular-rotas-por-estrada)
8. [Análise Solar e Lunar](#8-análise-solar-e-lunar)
9. [Análise por Inteligência Artificial](#9-análise-por-inteligência-artificial)
10. [Trabalhar Offline (Sem Internet)](#10-trabalhar-offline-sem-internet)
11. [Guardar e Partilhar (Importar/Exportar)](#11-guardar-e-partilhar-importarexportar)
12. [Gerar Relatórios](#12-gerar-relatórios)
13. [Capturar Imagem do Mapa](#13-capturar-imagem-do-mapa)
14. [Desfazer Acções](#14-desfazer-acções)
15. [Atalhos Rápidos](#15-atalhos-rápidos)
16. [Usar em Telemóvel ou Tablet](#16-usar-em-telemóvel-ou-tablet)
17. [Personalização Visual](#17-personalização-visual)
18. [Dicas e Boas Práticas](#18-dicas-e-boas-práticas)
19. [Resolver Problemas Comuns](#19-resolver-problemas-comuns)
20. [Fluxo Recomendado para Nova Operação](#20-fluxo-recomendado-para-nova-operação)

---

## 1. Primeiros Passos

### Escolher o Perfil Operacional

Quando abres a plataforma pela primeira vez, aparece um ecrã com dois perfis:

- **GIOE** — Grupo de Intervenção de Operações Especiais (cor vermelha)
- **ISEOP** — Intervenção em Situações Especiais de Ordem Pública (cor verde)

Clica naquele que corresponde à tua unidade. Esta escolha:
- Define a cor que aparece nos relatórios, barreiras e perímetros
- Personaliza o branding em PDFs, Word e capturas
- Fica memorizada para próximas sessões

### Mudar de Perfil

Podes alternar entre perfis a qualquer momento — clica no nome do perfil no canto inferior direito da barra de status. **Não perdes os teus pontos** ao mudar; só as cores e o nome nos relatórios mudam.

---

## 2. Navegar no Mapa

### Movimentação Básica
- **Arrastar com rato** → mover o mapa
- **Roda do rato** ou **`+` / `−`** no canto superior esquerdo → ampliar / reduzir
- **Duplo clique** → zoom no ponto clicado

### Mudar Tipo de Mapa
No painel lateral encontras 13 estilos de mapa diferentes, agrupados:

- **Google**: Satélite, Híbrido (satélite + nomes), Terreno, Ruas
- **ESRI**: World Imagery, Topográfico, Streets
- **Bing**: Aéreo
- **Open-source**: OpenStreetMap, OpenTopoMap, CartoDB Dark, CartoDB Light, OSM França (edifícios)

Clica numa miniatura para mudar imediatamente.

**Recomendado:**
- **Satélite Google** para análise visual de zonas
- **OpenTopoMap** para terrenos com relevo (montanhas, vales)
- **CartoDB Dark** para vista nocturna com bom contraste

### Escala
No canto inferior esquerdo aparece sempre uma escala em metros/km que se actualiza com o zoom — ajuda a estimar distâncias rapidamente.

### Posição inicial
O mapa abre por defeito centrado em Loures (38.76, -9.20). Podes começar a navegar a partir daí.

---

## 3. Marcar Pontos Tácticos

A plataforma tem **29 tipos de marcadores** organizados por categoria.

### Como Criar um Ponto

**Método 1 — Toolbar:**
1. Clica no botão "Marker" (alfinete) na barra superior
2. Clica no mapa onde queres marcar
3. Edita os campos no painel lateral

**Método 2 — Botão direito:**
1. Botão direito sobre o mapa
2. Escolhe **"⊕ Fixar ponto aqui"**

### Tipos Disponíveis

**Navegação e Posição** (azul)
- WPT — Waypoint genérico
- OP — Posto de observação
- BP — Posição de batalha
- CP — Checkpoint

**Alvos e Suspeitos** (vermelho/laranja)
- TGT — Alvo confirmado
- SUS — Suspeito
- HOS — Refém / Hostage
- VIP — Pessoa de interesse / VIP

**Equipas Amigas**
- FRP — Equipa amiga genérica
- **PC** — Posto de Comando (azul)
- **PAT** — Patrulha GNR (verde escuro)
- **GIO** — Equipa GIOE (vermelho com **borda dourada**)
- **GIP** — Equipa GIOP (preto com **borda dourada**)
- SNP — Sniper
- STK — Stack
- BRE — Breacher
- K9 — Equipa cinotécnica
- EOD — Desactivação de explosivos
- NEG — Negociador
- DRN — Drone

**Objectivos e Acção**
- OBJ — Objectivo
- INF — Infiltração
- EXF — Exfiltração

**Logística e Comunicações**
- CCP — Casualty Collection Point
- SUP — Suporte logístico
- COM — Comunicações
- HLZ — Zona de aterragem helicóptero

**Viaturas**
- VEH — Viatura genérica
- TVE — Viatura táctica

**Perigo**
- HZD — Risco / Hazard

### Personalizar Cada Ponto

Em cada marcador podes definir:
- **Nome** (ex: "Casa do alvo principal")
- **Descrição** e **notas**
- **Prioridade**: Alta / Média / Baixa — Alta mostra um ponto vermelho pulsante
- **Estado**: Planeado / Activo / Comprometido / Neutralizado
  - Planeado → marcador tracejado
  - Comprometido → X vermelho sobreposto
  - Neutralizado → opacidade reduzida
- **Confiança**: Alta / Média / Baixa — mostra "?" amarelo ou vermelho

### Ver Detalhes de um Ponto

Clica num marcador → aparece um popup com:
- Coordenadas em formato decimal e UTM
- **Altitude** (obtida automaticamente)
- Prioridade e descrição
- Botões de acção:
  - **▶ ROTA DAQUI** (verde fluorescente) — calcula rota desde a tua posição GPS
  - **EDITAR** — abre formulário no painel
  - **CENTRAR** — centra o mapa nesse ponto
  - **✕ REMOVER** — apaga (com confirmação via undo)

### Mover ou Editar
- **Arrasta** o marcador com o rato para reposicionar
- **Botão direito** sobre o marcador → menu com:
  - Editar
  - Remover
  - Centrar mapa
  - Rota da minha posição até aqui (se GPS estiver activo)
  - Abrir no Google Maps

---

## 4. Fazer Medições

Ferramentas disponíveis na barra superior. Após escolher uma ferramenta, aparece uma **dica na barra inferior** a explicar o que fazer.

### Distância (régua)
1. Clica no botão da régua
2. Clica em vários pontos no mapa
3. **Duplo-clique** ou **Enter** para terminar
4. Mostra distância de cada segmento e total
5. Cor: amarelo fluorescente

### Área
1. Clica no botão de polígono
2. Clica nos vértices da área
3. **Duplo-clique** para fechar e calcular
4. Apresenta área em m² ou km² automaticamente

### Raio / Círculo
1. Primeiro clique = centro
2. Segundo clique = define o raio
3. Útil para áreas de cobertura, raios de operação
4. Cor: ciano fluorescente

### Azimute
1. Primeiro clique = origem
2. Segundo clique = destino
3. Mostra ângulo (0-360°) e distância
4. Cor: verde fluorescente

### Anéis de Alcance
- Clica no centro
- Desenha automaticamente **3 anéis** a 500m / 1km / 2km
- Útil para visualizar perímetros de protecção

### Sector de Tiro
1. Primeiro clique = posição
2. Segundo clique = direcção e alcance
3. Desenha um cone de 60° na direcção indicada
4. Cor: laranja

### Rota Multi-Segmento
1. Clica em vários waypoints sequenciais
2. **Duplo-clique** ou **Enter** para terminar
3. Calcula distância total

### Zona de Exclusão / Buffer
1. Centro + raio
2. Visual distintivo: tracejado vermelho
3. Útil para áreas de risco

### Barreira / Corte de Estrada
1. Clica nas duas extremidades (A e B) do corte
2. Desenha um rectângulo escuro estreito perpendicular
3. Mostra o comprimento
4. Útil para sinalizar acessos bloqueados, cortes de estrada

### Quadrícula Militar (MGRS)
- Botão dedicado ou tecla `Q`
- Liga/desliga uma grelha sobre o mapa com referências MGRS de 1km
- Compatível com cartografia militar standard

### Limpar Tudo
- Botão "Clear" na toolbar
- Remove **todas** as medições de uma vez
- Reversível com Ctrl+Z

---

## 5. Adicionar Comentários

Caixas de texto em formato de balão de fala, sempre visíveis no mapa.

### Como Criar
1. Clica no botão "Caixa de Comentário" (cor amarela na toolbar)
2. Clica no mapa onde queres colocar
3. Aparece um modal com:
   - Campo de texto (máx. **80 caracteres**)
   - Contador de caracteres
   - **3 cores** disponíveis:
     - **Branco** (fundo branco, texto preto, borda preta)
     - **Preto** (fundo preto, texto branco, borda branca)
     - **Vermelho** (fundo vermelho, texto branco, borda branca)
4. Escreve o texto, escolhe a cor, clica **Guardar**

### Editar
- **Clique** sobre o balão → reabre o modal
- Podes mudar texto e/ou cor
- Apagar todo o texto = remove o balão

### Mover
- **Arrasta** o balão para reposicionar

### Apagar
- **Botão direito** → "✕ Remover"

### Casos de Uso Típicos
- "ZONA DE REUNIÃO" sobre área de concentração
- "Acesso bloqueado por obras"
- "Câmara de vigilância"
- "Hora H+30 reagrupar aqui"
- "Estacionamento de viaturas"

Os balões aparecem nas capturas PNG e relatórios.

---

## 6. Usar o GPS

Dois botões no canto superior direito do mapa.

### Botão Principal (alvo)
- **Toque curto** → fixa a tua posição actual uma vez (mostra ponto azul pulsante + círculo de precisão)
- **Toque longo (manter pressionado ~1 segundo)** → modo tracking contínuo, segue-te em tempo real e desenha o teu percurso

### Botão "Marcar a Minha Posição"
- Cria automaticamente um marcador WPT na tua posição actual
- Nome automático: `GPS-HHMM` (hora actual)

### O Que Vês
- **Ponto azul pulsante** na tua localização
- **Círculo à volta** = margem de precisão (em metros)
- **Tooltip** com altitude, velocidade (km/h) e direcção

### Na Barra de Status
Quando o GPS está activo e há pontos no mapa, aparece:
> → NOME_PONTO 245m / 87°

Indica o **ponto táctico mais próximo**, distância e direcção.

### Importante Saber
- O browser pede permissão na primeira vez — aceita
- Em **smartphone/tablet** com vista para o céu: precisão de 5-15m
- Em **desktop sem GPS**: precisão pode ser de centenas de metros (usa Wi-Fi/IP)
- Se mudares de separador e voltares, o GPS retoma automaticamente sem novo pedido de permissão

---

## 7. Calcular Rotas por Estrada

A plataforma usa **OpenRouteService** para calcular rotas reais por estrada.

### Configuração Inicial (uma vez)
1. Vai a [openrouteservice.org/dev](https://openrouteservice.org/dev)
2. Cria conta gratuita
3. Copia a tua **API key**
4. Na plataforma, **botão direito** sobre o botão de routing (verde fluorescente na toolbar)
5. Cola a chave e guarda

**Limite gratuito:** 1.000 rotas/dia (mais do que suficiente para uso normal).

### Calcular uma Rota

**Método 1 — Entre dois pontos quaisquer:**
1. Clica no botão de routing
2. Clica no ponto A
3. Clica no ponto B
4. Rota calculada e desenhada automaticamente

**Método 2 — Da minha posição GPS até um marcador:**
1. Activa o GPS (toque no botão GPS no canto)
2. Clica num marcador qualquer
3. No popup, clica em **"▶ ROTA DAQUI"** (botão verde fluorescente)
4. Rota desde GPS até esse ponto, calculada e centrada no mapa

### O Que Vês
- Linha verde fluorescente no caminho
- Marcadores A (verde) e B (vermelho) nas extremidades
- Etiqueta no meio: **"X km · Y min"**
- Mapa centra-se automaticamente para mostrar toda a rota

### Exportar/Importar Chave
No popover da chave podes:
- **Exportar** chave em ficheiro `.json` (para usar noutro dispositivo)
- **Importar** chave a partir de ficheiro

### Mensagens de Erro
- "Sem ligação à API" → verifica internet ou chave
- "Chave inválida ou bloqueada" → re-verifica em openrouteservice.org
- "Limite diário excedido" → atingiste 1000/dia, espera até amanhã
- "Não encontrou rota" → pontos sem estradas acessíveis entre eles (ilha, deserto, etc.)

---

## 8. Análise Solar e Lunar

Saber posição do sol/lua, horários crepusculares, fases lunares.

### Como Abrir
- Botão "☀" na toolbar (cor ciano)
- Atalho de teclado: **`L`**

### Informação Apresentada

**Sol:**
- Hora do **nascer-do-sol**
- Hora do **pôr-do-sol**
- **Zénite** (sol no ponto mais alto)
- **Azimute actual** (em que direcção está)
- **Elevação** (altura no céu, em graus)
- **Duração do dia**

**Lua:**
- Nascer e pôr da lua
- **Fase actual** (Nova, Crescente, Quarto Crescente, Cheia, Minguante, etc.)
- **Iluminação** (% de superfície visível)

**Crepúsculos militares:**
- **BMNT** (Beginning Morning Nautical Twilight): astronómico (-18°), náutico (-12°), civil (-6°)
- **EENT** (End Evening Nautical Twilight): civil, náutico, astronómico

### Simular Outras Horas

Útil para planear operações em horários específicos.

- **Slider** de 0 a 1439 minutos (de 00:00 a 23:55, em incrementos de 5 min)
- **Botões rápidos**:
  - **⏱ Hora actual**
  - **☀ Nascer** (salta para o nascer-do-sol de hoje)
  - **☾ Pôr** (salta para o pôr-do-sol)
  - **☼ Zénite** (salta para meio-dia solar)
- Quando movimentas o slider, **todos os valores recalculam em tempo real**
- Indicador grande mostra:
  - "AGORA · 14:32" (verde) → modo real-time
  - "SIMULADO · 06:15" (âmbar) → modo simulação

### Projectar no Mapa

Botão **"Projectar no mapa"** dentro do painel desenha 3 linhas radiais a partir do centro do mapa:

- **Linha tracejada âmbar** — direcção do nascer-do-sol
- **Linha tracejada laranja** — direcção do pôr-do-sol
- **Linha sólida amarela** — sol actual (apenas se acima do horizonte)

Etiquetas dos valores em **branco fluorescente** para legibilidade. Em modo simulação, as linhas actualizam-se com a hora simulada.

---

## 9. Análise por Inteligência Artificial

Identifica automaticamente objectos visíveis no mapa (viaturas, edifícios, pessoas, etc.).

### Como Configurar
- Botão "🔍" na toolbar (cor ciano)
- Atalho: **`I`**
- Escolhe um dos 5 providers e cola a chave gratuita:
  - **Gemini** (Google) — gratuito, recomendado para começar
  - **Groq** (LLaMA Vision) — gratuito, muito rápido
  - **Mistral Pixtral** — gratuito
  - **OpenRouter** — múltiplos modelos
  - **Claude** (Anthropic)

### Como Usar
1. Configura tipos de objectos a procurar (viaturas, edifícios, pessoas...)
2. Clica **"Iniciar Scan"**
3. A IA analisa a vista actual do mapa
4. Aparecem caixas coloridas a destacar cada objecto detectado
5. Painel lateral mostra lista com nível de confiança
6. Podes converter qualquer detecção em ponto táctico oficial

As chaves API ficam guardadas localmente — não precisas de re-introduzir.

---

## 10. Trabalhar Offline (Sem Internet)

A plataforma continua a funcionar sem internet — desde que tenhas pré-descarregado os tiles de mapa que precisas.

### Cache Automática

Tudo o que vês durante o uso normal é **automaticamente guardado**. Se voltares offline depois, esses pedaços de mapa continuam a aparecer.

Indicador no canto inferior:
- 🟢 **ONLINE** (verde) — tens internet
- 🔴 **OFFLINE** (vermelho pulsante) — sem internet

Contador "CACHE: N" mostra quantos pedaços de mapa tens guardados.

### Descarregar uma Área para Uso Offline

Para preparar uma operação onde sabes que não vais ter internet:

1. Clica no botão **"Download Área"** na toolbar (cor ciano, ícone de seta para baixo)
2. **Clica e arrasta** no mapa para desenhar um rectângulo na área que queres
3. Aparece um modal com:
   - Tamanho da área seleccionada
   - **Slider zoom mínimo / máximo** (recomendado: 13-17 para uso urbano, 11-14 para áreas extensas)
   - **6 tipos de mapa** seleccionáveis (apenas open-source — Google e Bing não são permitidos descarregar em massa)
   - **Estimativa**: número de tiles + MB
   - Aviso a vermelho se for muito grande (>50.000 tiles)
4. Clica **"Iniciar Download"**
5. Modal de progresso mostra X / Y, velocidade
6. Podes cancelar a meio (o que já foi guardado mantém-se)

### Limpar Cache

Botão vermelho "Limpar Cache" — apaga **todos** os tiles guardados (com confirmação).

### O Que Funciona Offline
- Navegação no mapa (áreas em cache)
- Criar/editar pontos tácticos
- Fazer medições
- Adicionar comentários
- Guardar e exportar KMZ/KML
- Gerar relatórios PDF e Word

### O Que Não Funciona Offline
- AI Scan (precisa do servidor de IA)
- Routing ORS (precisa do OpenRouteService)
- Pesquisa de moradas
- Altitude automática

---

## 11. Guardar e Partilhar (Importar/Exportar)

### KMZ / KML

**Formato universal** compatível com Google Earth, Google Maps, QGIS, ATAK, JCATS, e qualquer software cartográfico moderno.

**Exportar:**
- Botão verde **"↓ KMZ"** ou **"↓ KML"** na toolbar
- Gera um ficheiro com **todos os pontos, medições e comentários** organizados em pastas

**Importar:**
- Botão azul **"↑ KMZ"** na toolbar
- Selecciona ficheiro `.kmz` ou `.kml`
- Pontos e medições aparecem no mapa imediatamente

### Persistência Automática

Tudo o que fazes é **guardado automaticamente** no teu browser. Se fechares acidentalmente:
- Reabre a plataforma
- Aparece prompt: *"Foi encontrado trabalho não guardado (há X minutos): N pontos, M medições, K notas. Queres restaurar?"*
- Aceita → tudo volta exactamente como estava

---

## 12. Gerar Relatórios

A plataforma gera relatórios profissionais com a tua identidade GIOE/ISEOP automaticamente aplicada.

### Relatório de Missão (PDF Completo)

Botão **"↓ RELATÓRIO COMPLETO + MAPA PDF"** no painel lateral. Gera 7 páginas:

1. **Capa** — banner colorido do perfil, classificação SEGNAC, data e hora
2. **Sumário Executivo** — número de pontos, medições, alvos, prioridades
3. **Captura do Mapa** — imagem alta resolução com tudo o que está visível
4. **Tabela de Pontos** — designação, tipo, coordenadas, prioridade, estado, notas
5. **Medições** — distâncias, áreas, raios, etc.
6. **Análise IA** (se houver detecções)
7. **Aprovação** — 3 linhas para assinaturas (Operador, Comandante, Comando)

### Ficha de Alvo (PDF)

Botão **"↓ FICHA PDF"** no painel do alvo seleccionado.

Específico para tipo TGT, inclui:
- Identificação do alvo
- Nível de ameaça (CRÍTICO/ALTO/MÉDIO/BAIXO) com cor
- Inteligência disponível
- **ROE** (Rules of Engagement)
- Janela operacional
- Aprovação com 3 assinaturas
- Aviso de classificação SEGNAC 1

### Versão Word (`.doc`)

Ao lado dos botões PDF tens **"↓ WORD"** — gera o mesmo conteúdo em formato editável.

Vantagens do Word:
- Podes **editar** depois (adicionar parágrafos, comentários)
- Abre no MS Word, LibreOffice, Google Docs
- Útil para revisão por superiores antes de imprimir

### Personalização Automática

| Elemento | GIOE | ISEOP |
|---|---|---|
| Cor do banner | Vermelho | Verde |
| Logo grande | "GIOE" | "ISEOP" |
| Subtítulo | "Grupo de Intervenção de Operações Especiais" | "Intervenção em Situações Especiais de Ordem Pública" |
| Nome do ficheiro | `GIOE_RelMissao_NOME_DATA.pdf` | `ISEOP_...` |

---

## 13. Capturar Imagem do Mapa

Botão verde com ícone de **câmara fotográfica** na toolbar.

### O Que Faz
Tira uma "fotografia" da vista actual do mapa em **alta resolução**, incluindo:
- Mapa base (qualquer tipo)
- Todos os pontos tácticos
- Todas as medições
- Caixas de comentário
- Quadrícula MGRS (se activa)
- GPS marker (se activo)
- Rotas calculadas

### Resolução
- **Triplica a resolução do ecrã** — num ecrã 1920×1080 obtém 5760×3240 pixels (qualidade ~6K)
- Texto e linhas extra-nítidas
- Formato PNG, máxima qualidade

### Output
- Ficheiro descarrega automaticamente: `GIOE_MapaCaptura_DATA-HORA.png`
- Captura **pura**, sem watermarks ou banners
- Pronto para usar em apresentações, briefings, anexos a relatórios

---

## 14. Desfazer Acções

A plataforma guarda as últimas **30 acções** que fizeste.

### Como Desfazer
- **Ctrl+Z** (Windows/Linux) ou **Cmd+Z** (Mac)
- Botão "Undo" (seta) na toolbar

### O Que Pode Ser Desfeito
- Criar ponto
- Editar ponto
- Eliminar ponto
- Adicionar medição
- Limpar todas as medições
- Criar/editar/eliminar comentário
- Mover marker

### Notificação
Cada desfazer mostra: *"✓ Desfeito"* ou nome da acção que reverteu.

---

## 15. Atalhos Rápidos

| Tecla | Acção |
|---|---|
| **Ctrl+Z** / **Cmd+Z** | Desfazer última acção |
| **Q** | Mostrar/ocultar quadrícula MGRS |
| **O** | Activar ferramenta de routing |
| **L** | Abrir painel Sol/Lua |
| **I** | Abrir AI Scan |
| **TAB** | Mostrar/ocultar painel lateral |
| **Enter** | Terminar medição em curso (régua, área, rota) |
| **Esc** | Cancelar acção em curso |

---

## 16. Usar em Telemóvel ou Tablet

A plataforma funciona em qualquer dispositivo moderno.

### Em Telemóvel (ecrã pequeno)
- Sidebar e painel lateral aparecem como **overlays** sobre o mapa
- Botões mais espaçados para toque (40×40 pixels mínimo)
- Status bar mais compacta
- Botões "**☰ PONTOS**" e "**⊞ PAINEL**" no centro inferior para abrir/fechar

### Em Tablet (médio)
- Pode ser usado em **modo desktop** (interface completa)
- Ou activar **modo móvel** se preferires overlay (botão dedicado)

### Touchscreen
- **Toque** = clique
- **Toque longo** = botão direito do rato (menu de contexto)
- **Pinch** = zoom
- **Arrastar com 2 dedos** = pan

### GPS em Tablet/Telemóvel
Aproveita melhor o GPS verdadeiro do dispositivo:
- Precisão real de 5-15 metros (com céu visível)
- Útil para operadores no terreno
- Tracking contínuo segue-te em movimento

---

## 17. Personalização Visual

### Modo Escuro (default)
- Tons cinzentos neutros estilo Chrome Dark Mode
- Texto branco-suave
- Acentos coloridos por funcionalidade

### Modo Claro
- Toggle no canto da barra de status (ícone sol/lua)
- Cores claras para uso em ambiente bem iluminado

### Cores dos Botões da Toolbar (por categoria)
- **Cinzento** — ferramentas básicas (régua, área, círculo, etc.)
- **Âmbar** — objectos especiais (barreira, comentário)
- **Ciano** — utilitários (sol/lua, IA, download)
- **Verde fluorescente** — routing
- **Verde** — exportação (KMZ, KML, PNG)
- **Azul** — importação
- **Vermelho** — acções destrutivas (limpar)

---

## 18. Dicas e Boas Práticas

### Para Planeamento
1. Começa com **Satélite** para identificar a zona
2. Marca **TGT** (alvos), **OBJ** (objectivos), **HZD** (perigos) primeiro
3. Adiciona **WPT** ou **CP** para pontos de passagem
4. Usa **medições** (distâncias, raios) para validar planos
5. Adiciona **comentários** com informação contextual
6. Gera **PDF de relatório** para briefing

### Para Operação no Terreno
1. **Antes de sair** (com internet): descarrega a área da operação para offline
2. **Activa o GPS** ao chegar
3. Usa **toque longo** no GPS para tracking contínuo
4. **Marca posição** com o botão dedicado para criar WPT rápido
5. **Comentários** vermelhos para alertas, brancos para notas neutras
6. Antes de regressar: **captura PNG** da situação final

### Para Briefings
- Gera **PDF de Missão** com mapa de alta resolução
- Use **PNG** separado para slides/apresentações
- **Ficha de Alvo** específica para cada TGT crítico
- **Versão Word** se prevês edições antes de imprimir

### Para Partilhar com Outras Equipas
- Exporta em **KMZ** — abre em Google Earth, ATAK, qualquer plataforma
- Exporta também em **PDF** para revisão sem necessidade de software técnico
- Partilha **chave ORS** em formato JSON para terem o mesmo routing

---

## 19. Resolver Problemas Comuns

**O mapa fica cinzento ao mover:** Estás offline e essa área não foi descarregada. Volta para uma zona em cache ou liga internet.

**GPS pede permissão sempre:** Garante que estás em HTTPS. Em modo anónimo/incógnito, browsers nunca guardam permissões.

**Routing falha:** Verifica chave ORS (botão direito no botão de routing). Pode ter expirado ou atingiste o limite diário (1.000/dia).

**Captura PNG vem em branco:** Aguarda alguns segundos para os tiles carregarem antes de capturar. Não capturar imediatamente após mudar de tipo de mapa.

**Esqueci-me de guardar e fechei:** Reabre — vai aparecer prompt para restaurar (autosave guarda os últimos minutos automaticamente).

**Quero apagar tudo e começar do zero:** Limpa o cache do browser para o domínio, ou usa o botão "Limpar Cache" + remove pontos/medições manualmente.

---

## 20. Fluxo Recomendado para Nova Operação

1. **Selecciona perfil** (GIOE / ISEOP)
2. **Navega** até à zona da operação no mapa
3. **Descarrega área** para offline (se vais para o terreno)
4. **Cria pontos tácticos** começando pelos críticos (TGT, OBJ)
5. **Adiciona medições** (distâncias, raios de cobertura)
6. **Anota comentários** sobre observações
7. **Confere posição solar** se relevante para timing
8. **Gera relatório PDF** ou **captura PNG**
9. **Exporta KMZ** para partilhar com outras equipas
10. **Sai com confiança** — tudo está autogravado

---

*Plataforma desenvolvida por CO/DI/CI — FJCC, para apoiar análise táctica e o planeamento operacional.*
