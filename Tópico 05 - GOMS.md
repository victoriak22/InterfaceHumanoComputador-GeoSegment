# Modelos GOMS – GeoSegment

Este documento reúne os modelos GOMS (Goals, Operators, Methods, Selection rules) por persona, alinhados às HTA do Tópico 05.

## Sumário

- [GOMS — HTA 1 (Ricardo Mendes)](#goms--hta-1-ricardo-mendes)
- [GOMS — HTA 2 (Dra. Helena Silveira)](#goms--hta-2-dra-helena-silveira)
- [GOMS — HTA 3 (Felipe Antunes)](#goms--hta-3-felipe-antunes)
- [GOMS — HTA 4 (Cláudia Torres)](#goms--hta-4-cláudia-torres)
- [GOMS — HTA 5 (Sr. Benedito)](#goms--hta-5-sr-benedito)

---

## GOMS — HTA 1 (Ricardo Mendes)

### Modelo GOMS – Analisar uso do solo a partir de imagem aérea

#### GOAL 0: analisar uso do solo a partir de imagem aérea

---

#### GOAL 1: carregar imagem da área de interesse

**METHOD 1.A: carregar imagem local**  
*(SEL. RULE: usuário possui a imagem salva no computador)*

- **OP. 1.A.1:** deslocar o cursor do mouse até o botão "Selecionar imagem"
- **OP. 1.A.2:** clicar com o botão esquerdo do mouse
- **OP. 1.A.3:** navegar até o diretório da imagem
- **OP. 1.A.4:** selecionar arquivo no formato `.tiff` ou `.png`
- **OP. 1.A.5:** confirmar seleção do arquivo
- **OP. 1.A.6:** verificar pré-visualização da imagem carregada

**METHOD 1.B: substituir imagem carregada**  
*(SEL. RULE: usuário identifica erro ou deseja trocar a imagem)*

- **OP. 1.B.1:** clicar no botão "Cancelar/Substituir imagem"
- **OP. 1.B.2:** retornar ao seletor de arquivos
- **OP. 1.B.3:** repetir operações do METHOD 1.A

---

#### GOAL 2: configurar segmentação automática

**METHOD 2.A: configurar usando parâmetros padrão**  
*(SEL. RULE: usuário não especialista ou deseja análise rápida)*

- **OP. 2.A.1:** examinar descrição resumida dos modelos disponíveis
- **OP. 2.A.2:** selecionar modelo padrão (ex.: V0)
- **OP. 2.A.3:** manter parâmetros de execução sugeridos pelo sistema

**METHOD 2.B: configurar usando parâmetros personalizados**  
*(SEL. RULE: usuário especialista ou deseja maior precisão)*

- **OP. 2.B.1:** selecionar modelo avançado (V1 ou V2)
- **OP. 2.B.2:** ajustar parâmetros de execução
- **OP. 2.B.3:** confirmar configurações escolhidas

---

#### GOAL 3: executar segmentação automática

- **OP. 3.A.1:** deslocar o cursor até o botão "Executar segmentação"
- **OP. 3.A.2:** clicar com o botão esquerdo do mouse
- **OP. 3.A.3:** acompanhar barra de progresso
- **OP. 3.A.4:** examinar mensagem de conclusão do processamento

---

#### GOAL 4: visualizar resultados da segmentação

- **OP. 4.A.1:** abrir painel de visualização de mapas
- **OP. 4.A.2:** ativar visualização lado a lado
- **OP. 4.A.3:** aplicar zoom no mapa
- **OP. 4.A.4:** alternar camadas de visualização
- **OP. 4.A.5:** verificar coerência espacial da segmentação

#### GOAL 4.1: Analisar estatísticas

**METHOD 4.1.A: analisar estatísticas por classe**  
*(SEL. RULE: foco em análise quantitativa do uso do solo)*

- **OP. 4.1.A.1:** acessar painel de estatísticas
- **OP. 4.1.A.2:** examinar percentuais por classe
- **OP. 4.1.A.3:** comparar distribuição das classes
- **OP. 4.1.A.4:** interpretar resultados numéricos

**METHOD 4.1.B: analisar estatísticas por histórico**  
*(SEL. RULE: dados de múltiplas execuções ou períodos disponíveis)*

- **OP. 4.1.B.1:** selecionar período ou execução anterior
- **OP. 4.1.B.2:** comparar variações nas classes de uso do solo
- **OP. 4.1.B.3:** identificar tendências ou mudanças temporais

---

## GOMS — HTA 2 (Dra. Helena Silveira)

### Modelo GOMS – Avaliar desempenho dos modelos de segmentação

#### GOAL 0: avaliar desempenho dos modelos de segmentação

---

#### GOAL 1: carregar conjunto de imagens de teste

**METHOD 1.A: carregar patches de validação manualmente**  
*(SEL. RULE: usuário possui conjunto de imagens de validação local)*

- **OP. 1.A.1:** deslocar o cursor do mouse até o botão "Selecionar imagens"
- **OP. 1.A.2:** clicar com o botão esquerdo do mouse
- **OP. 1.A.3:** navegar até o diretório contendo os patches de validação
- **OP. 1.A.4:** selecionar arquivos de imagem (ex.: .tiff ou .png)
- **OP. 1.A.5:** confirmar seleção dos arquivos
- **OP. 1.A.6:** verificar lista de imagens carregadas no sistema

**METHOD 1.B: carregar dataset em lote**  
*(SEL. RULE: usuário possui grande quantidade de imagens de validação)*

- **OP. 1.B.1:** selecionar opção "Upload em lote"
- **OP. 1.B.2:** selecionar múltiplos arquivos ou pasta de imagens
- **OP. 1.B.3:** confirmar envio do dataset
- **OP. 1.B.4:** verificar lista completa de arquivos enviados

---

#### GOAL 2: selecionar arquitetura de modelo

**METHOD 2.A: selecionar modelo diretamente**  
*(SEL. RULE: usuário já conhece o modelo que deseja testar)*

- **OP. 2.A.1:** examinar lista de arquiteturas disponíveis
- **OP. 2.A.2:** selecionar modelo desejado (V0, V1 ou V2)
- **OP. 2.A.3:** confirmar seleção da arquitetura

**METHOD 2.B: comparar modelos antes de selecionar**  
*(SEL. RULE: usuário deseja analisar métricas antes da escolha)*

- **OP. 2.B.1:** examinar descrição da arquitetura do modelo
- **OP. 2.B.2:** visualizar métricas resumidas do modelo
- **OP. 2.B.3:** comparar desempenho entre modelos disponíveis
- **OP. 2.B.4:** selecionar modelo mais adequado para o experimento

---

#### GOAL 3: executar segmentação automática

- **OP. 3.A.1:** deslocar cursor até o botão "Executar segmentação"
- **OP. 3.A.2:** clicar com o botão esquerdo do mouse
- **OP. 3.A.3:** acompanhar barra de progresso do processamento
- **OP. 3.A.4:** examinar mensagem de conclusão da inferência

---

#### GOAL 4: analisar resultados da segmentação

- **OP. 4.A.1:** abrir painel de resultados da segmentação
- **OP. 4.A.2:** visualizar mapas segmentados gerados pelo modelo
- **OP. 4.A.3:** aplicar zoom em regiões específicas da imagem
- **OP. 4.A.4:** verificar coerência visual das classes segmentadas

---

#### GOAL 4.1: comparar métricas de desempenho

**METHOD 4.1.A: analisar métricas quantitativas**  
*(SEL. RULE: foco em avaliação quantitativa do desempenho do modelo)*

- **OP. 4.1.A.1:** acessar painel de métricas de desempenho
- **OP. 4.1.A.2:** examinar valor de mIoU global
- **OP. 4.1.A.3:** examinar IoU por classe
- **OP. 4.1.A.4:** comparar resultados com experimentos anteriores

---

#### GOAL 4.2: avaliar qualidade visual da segmentação

**METHOD 4.2.A: avaliar refinamento das bordas**  
*(SEL. RULE: foco em avaliação qualitativa da segmentação)*

- **OP. 4.2.A.1:** visualizar bordas das regiões segmentadas
- **OP. 4.2.A.2:** aplicar zoom em áreas de interesse
- **OP. 4.2.A.3:** examinar precisão das fronteiras entre classes
- **OP. 4.2.A.4:** identificar possíveis erros de segmentação

---

## GOMS — HTA 3 (Felipe Antunes)

### Modelo GOMS – Gerar dados de cobertura vegetal para relatórios ambientais

#### GOAL 0: gerar dados de cobertura vegetal para relatórios ambientais

---

#### GOAL 1: acessar o sistema

**METHOD 1.A: acessar usando credenciais**  
*(SEL. RULE: usuário possui login e senha cadastrados)*

- **OP. 1.A.1:** deslocar o cursor até o campo de login
- **OP. 1.A.2:** digitar nome de usuário ou e-mail
- **OP. 1.A.3:** deslocar o cursor até o campo de senha
- **OP. 1.A.4:** digitar senha de acesso
- **OP. 1.A.5:** clicar no botão "Entrar"
- **OP. 1.A.6:** verificar carregamento do dashboard do sistema

**METHOD 1.B: acessar histórico de análises**  
*(SEL. RULE: usuário deseja reutilizar ou revisar processamento anterior)*

- **OP. 1.B.1:** acessar painel de histórico
- **OP. 1.B.2:** examinar lista de análises anteriores
- **OP. 1.B.3:** selecionar análise desejada

---

#### GOAL 2: carregar imagens da área de interesse

**METHOD 2.A: carregar imagem local**  
*(SEL. RULE: imagem está armazenada no computador do usuário)*

- **OP. 2.A.1:** deslocar cursor até botão "Selecionar imagem"
- **OP. 2.A.2:** clicar no botão esquerdo do mouse
- **OP. 2.A.3:** navegar até o diretório da imagem
- **OP. 2.A.4:** selecionar arquivo de imagem (ex.: ortofoto ou recorte de satélite)
- **OP. 2.A.5:** confirmar seleção do arquivo
- **OP. 2.A.6:** verificar pré-visualização da imagem carregada

**METHOD 2.B: substituir imagem enviada**  
*(SEL. RULE: usuário percebe erro ou deseja analisar outra área)*

- **OP. 2.B.1:** clicar no botão "Substituir imagem"
- **OP. 2.B.2:** retornar ao seletor de arquivos
- **OP. 2.B.3:** repetir operações do METHOD 2.A

---

#### GOAL 3: executar segmentação automática

- **OP. 3.A.1:** deslocar cursor até botão "Executar segmentação"
- **OP. 3.A.2:** clicar com botão esquerdo do mouse
- **OP. 3.A.3:** acompanhar barra de progresso do processamento
- **OP. 3.A.4:** examinar mensagem de conclusão da segmentação

---

#### GOAL 4: obter resultados da segmentação

- **OP. 4.A.1:** abrir painel de resultados
- **OP. 4.A.2:** visualizar mapa segmentado
- **OP. 4.A.3:** aplicar zoom em regiões específicas da imagem
- **OP. 4.A.4:** verificar coerência das classes identificadas

---

#### GOAL 4.1: analisar estatísticas

**METHOD 4.1.A: examinar estatísticas por classe**  
*(SEL. RULE: usuário precisa avaliar proporção das classes detectadas)*

- **OP. 4.1.A.1:** acessar painel de estatísticas
- **OP. 4.1.A.2:** examinar percentuais de cada classe
- **OP. 4.1.A.3:** interpretar distribuição das classes de uso do solo

**METHOD 4.1.B: copiar dados para relatório**  
*(SEL. RULE: usuário precisa incluir dados em relatório técnico)*

- **OP. 4.1.B.1:** selecionar tabela de estatísticas
- **OP. 4.1.B.2:** copiar valores exibidos
- **OP. 4.1.B.3:** inserir dados em planilha ou documento técnico

---

#### GOAL 5: exportar resultados

**METHOD 5.A: exportar mapa segmentado**  
*(SEL. RULE: usuário precisa do mapa para relatório ambiental)*

- **OP. 5.A.1:** clicar no botão "Exportar mapa"
- **OP. 5.A.2:** selecionar formato de saída (PNG ou GeoTIFF)
- **OP. 5.A.3:** confirmar download do arquivo

**METHOD 5.B: exportar estatísticas**  
*(SEL. RULE: usuário precisa dos dados para análise quantitativa)*

- **OP. 5.B.1:** clicar no botão "Exportar estatísticas"
- **OP. 5.B.2:** selecionar formato de saída (CSV ou planilha)
- **OP. 5.B.3:** confirmar download do arquivo

---

## GOMS — HTA 4 (Cláudia Torres)

### Modelo GOMS – Avaliar dados de uso do solo para planejamento urbano

#### GOAL 0: avaliar dados de uso do solo para planejamento urbano

---

#### GOAL 1: acessar dashboard do sistema

**METHOD 1.A: acessar plataforma GeoSegment**  
*(SEL. RULE: usuário deseja iniciar nova análise ou consultar resultados disponíveis)*

- **OP. 1.A.1:** abrir navegador de internet
- **OP. 1.A.2:** digitar endereço da plataforma GeoSegment
- **OP. 1.A.3:** pressionar tecla Enter para carregar o sistema
- **OP. 1.A.4:** aguardar carregamento do dashboard

**METHOD 1.B: selecionar análise disponível**  
*(SEL. RULE: existem análises previamente executadas no sistema)*

- **OP. 1.B.1:** examinar lista de análises disponíveis no dashboard
- **OP. 1.B.2:** identificar análise relevante para planejamento urbano
- **OP. 1.B.3:** clicar na análise selecionada

---

#### GOAL 2: visualizar mapas temáticos

**METHOD 2.A: visualizar mapa segmentado**  
*(SEL. RULE: usuário deseja observar distribuição espacial das classes)*

- **OP. 2.A.1:** abrir painel de visualização de mapas
- **OP. 2.A.2:** ativar camada de mapa segmentado
- **OP. 2.A.3:** observar cores associadas às classes de uso do solo
- **OP. 2.A.4:** verificar legenda do mapa

**METHOD 2.B: comparar áreas urbanas e vegetação**  
*(SEL. RULE: usuário deseja analisar mudanças ou contrastes entre classes)*

- **OP. 2.B.1:** ativar visualização de múltiplas camadas
- **OP. 2.B.2:** alternar entre camadas de áreas urbanas e vegetação
- **OP. 2.B.3:** aplicar zoom em regiões de interesse
- **OP. 2.B.4:** observar diferenças espaciais entre classes

---

#### GOAL 3: analisar estatísticas

**METHOD 3.A: analisar estatísticas por histórico**  
*(SEL. RULE: existem dados de análises realizadas anteriormente)*

- **OP. 3.A.1:** acessar painel de estatísticas
- **OP. 3.A.2:** selecionar período ou análise anterior
- **OP. 3.A.3:** examinar evolução das classes de uso do solo
- **OP. 3.A.4:** identificar tendências ou mudanças temporais

**METHOD 3.B: analisar estatísticas por classe**  
*(SEL. RULE: usuário deseja avaliar distribuição atual das classes)*

- **OP. 3.B.1:** visualizar gráfico de distribuição das classes
- **OP. 3.B.2:** examinar percentuais de cada classe
- **OP. 3.B.3:** comparar proporção entre áreas urbanas, vegetação e outras classes
- **OP. 3.B.4:** interpretar resultados quantitativos

---

#### GOAL 4: apresentar resultados

**METHOD 4.A: apresentar resultados em reuniões**  
*(SEL. RULE: dados serão usados em decisões estratégicas ou planejamento urbano)*

- **OP. 4.A.1:** abrir painel de resumo da análise
- **OP. 4.A.2:** visualizar gráficos e mapas resumidos
- **OP. 4.A.3:** selecionar visualizações relevantes
- **OP. 4.A.4:** apresentar resultados para equipe ou gestores

**METHOD 4.B: gerar relatório visual**  
*(SEL. RULE: usuário precisa compartilhar resultados com outros setores)*

- **OP. 4.B.1:** clicar na opção "Gerar relatório"
- **OP. 4.B.2:** selecionar formato de relatório (PDF ou apresentação)
- **OP. 4.B.3:** confirmar geração do relatório
- **OP. 4.B.4:** realizar download do documento

---

## GOMS — HTA 5 (Sr. Benedito)

### Modelo GOMS – Verificar classificação da propriedade no mapa

#### GOAL 0: verificar classificação da propriedade no mapa

---

#### GOAL 1: acessar visualização do mapa

**METHOD 1.A: abrir sistema com ajuda de familiar**  
*(SEL. RULE: usuário possui pouca familiaridade com tecnologia)*

- **OP. 1.A.1:** solicitar ajuda do neto para acessar o sistema
- **OP. 1.A.2:** abrir navegador de internet no computador ou celular
- **OP. 1.A.3:** digitar endereço da plataforma GeoSegment
- **OP. 1.A.4:** pressionar Enter para carregar o sistema
- **OP. 1.A.5:** aguardar carregamento do mapa da plataforma

**METHOD 1.B: localizar propriedade no mapa**  
*(SEL. RULE: usuário deseja identificar sua propriedade no sistema)*

- **OP. 1.B.1:** acessar ferramenta de busca do mapa
- **OP. 1.B.2:** digitar endereço, coordenadas ou nome da propriedade
- **OP. 1.B.3:** selecionar resultado exibido pelo sistema
- **OP. 1.B.4:** centralizar mapa na área da propriedade

---

#### GOAL 2: verificar classificação da área

**METHOD 2.A: identificar área agrícola**  
*(SEL. RULE: usuário deseja verificar se sua área foi classificada corretamente)*

- **OP. 2.A.1:** observar cores das classes exibidas no mapa
- **OP. 2.A.2:** consultar legenda das classes de uso do solo
- **OP. 2.A.3:** identificar região correspondente à propriedade
- **OP. 2.A.4:** verificar se a área está classificada como agrícola

**METHOD 2.B: comparar classificação com situação real**  
*(SEL. RULE: usuário deseja confirmar se a classificação corresponde à realidade)*

- **OP. 2.B.1:** observar limites da área da propriedade
- **OP. 2.B.2:** comparar classificação exibida no mapa com uso real da terra
- **OP. 2.B.3:** verificar possíveis inconsistências na classificação

---

#### GOAL 3: confirmar resultado da classificação

**METHOD 3.A: verificar limites da propriedade**  
*(SEL. RULE: usuário deseja garantir que o sistema identificou corretamente sua área)*

- **OP. 3.A.1:** visualizar contorno da propriedade no mapa
- **OP. 3.A.2:** aplicar zoom para observar detalhes da área
- **OP. 3.A.3:** verificar se os limites correspondem à propriedade real

**METHOD 3.B: confirmar classificação da área**  
*(SEL. RULE: usuário deseja confirmar se a classificação exibida está correta)*

- **OP. 3.B.1:** examinar classe atribuída à área da propriedade
- **OP. 3.B.2:** verificar nível de confiança da classificação
- **OP. 3.B.3:** confirmar se o resultado corresponde à realidade observada