# Análise Hierárquica de Tarefas (HTA) – GeoSegment

Este documento descreve a Análise Hierárquica de Tarefas (HTA) do projeto GeoSegment, relacionando objetivos/operações com problemas e recomendações de usabilidade. As análises são baseadas nas personas definidas para o sistema, representando diferentes perfis de usuários e seus objetivos ao utilizar a plataforma, permitindo compreender como cada tipo de usuário interage com as funcionalidades do sistema.

## Sumário

- [HTA 1 — Ricardo Mendes (Fiscalização Ambiental)](#hta-1--ricardo-mendes-fiscalização-ambiental)
- [HTA 2 — Dra. Helena Silveira (Validação Científica)](#hta-2--dra-helena-silveira-validação-científica)
- [HTA 3 — Felipe Antunes (Consultor Ambiental)](#hta-3--felipe-antunes-consultor-ambiental)
- [HTA 4 — Cláudia Torres (Gestora Pública)](#hta-4--cláudia-torres-gestora-pública)
- [HTA 5 — Sr. Benedito (Proprietário Rural)](#hta-5--sr-benedito-proprietário-rural)

---

## Diagramas HTA

As estruturas hierárquicas das tarefas do sistema são representadas nos diagramas abaixo:

## **HTA 1 — Ricardo Mendes (Fiscalização Ambiental)**

<img width="1270" height="618" alt="image" src="https://github.com/user-attachments/assets/85b2a7cc-a9cd-4f7b-9424-671a2099e8b8" />


| Objetivos / Operações | Problemas e Recomendações |
|----------------------|---------------------------|
| **0. Analisar uso do solo a partir de imagem aérea (1 > 2 > 3 > 4)** | **Input:** imagem aérea de alta resolução (ex.: 30 cm/px) <br> **Feedback:** exibição do mapa segmentado e estatísticas por classe <br> **Plano:** carregar imagem → configurar segmentação → executar processamento → analisar resultados <br> **Recomendação:** permitir acesso via navegador sem necessidade de softwares especializados |
| **1. Carregar imagem da área de interesse (1.1 > 1.2)** | **Plano:** selecionar arquivo e confirmar upload <br> **Problema:** arquivos grandes podem gerar lentidão ou falhas <br> **Recomendação:** exibir barra de progresso e validação automática de formato e resolução |
| **1.1 Selecionar arquivo (.tiff ou .png)** | **Problema:** usuário pode tentar enviar formatos inválidos <br> **Recomendação:** restringir seleção apenas a formatos compatíveis |
| **1.2 Confirmar upload da imagem** | **Feedback:** pré-visualização da imagem carregada <br> **Recomendação:** permitir cancelamento ou substituição da imagem |
| **2. Configurar segmentação automática (2.1 > 2.2)** | **Plano:** selecionar modelo de IA e parâmetros de execução <br> **Problema:** usuários não especialistas podem não compreender termos técnicos <br> **Recomendação:** fornecer descrições simplificadas e tooltips |
| **2.1 Selecionar modelo de segmentação (V0, V1 ou V2)** | **Problema:** dificuldade em decidir qual modelo utilizar <br> **Recomendação:** apresentar métricas resumidas e indicação de uso recomendado |
| **2.2 Definir parâmetros de execução** | **Problema:** excesso de opções pode confundir usuários leigos <br> **Recomendação:** oferecer configurações padrão e modo avançado opcional |
| **3. Executar segmentação automática (depende de 1 e 2)** | **Ação:** iniciar processamento de inferência <br> **Problema:** tempo de espera elevado pode gerar ansiedade <br> **Recomendação:** exibir status do processamento e tempo estimado |
| **4. Visualizar resultados da segmentação (4.1 / 4.2)** | **Plano:** visualizar mapas e estatísticas simultaneamente <br> **Problema:** sobrecarga de informação visual <br> **Recomendação:** permitir personalização do dashboard |
| **4.1 Analisar estatísticas (4.1.1 / 4.1.2)** | **Problema:** dados numéricos podem ser difíceis de interpretar <br> **Recomendação:** uso de gráficos e percentuais simplificados |
| **4.1.1 Analisar estatísticas por histórico** | **Problema:** dificuldade em identificar mudanças ao longo do tempo <br> **Recomendação:** permitir comparação temporal quando disponível |
| **4.1.2 Analisar estatísticas por classe** | **Problema:** interpretação da distribuição das classes <br> **Recomendação:** destacar proporções por classe de uso do solo |
| **4.2 Visualizar mapas lado a lado** | **Feedback:** mapas coloridos facilitam a interpretação espacial <br> **Recomendação:** permitir zoom, sincronização e alternância de camadas |

--- 

## **HTA 2 — Dra. Helena Silveira (Validação Científica)**

<img width="1239" height="470" alt="image" src="https://github.com/user-attachments/assets/1723b8b8-148d-40d7-a785-a7c4c51a8543" />

| Objetivos / Operações | Problemas e Recomendações |
|---|---|
| **0. Avaliar desempenho dos modelos de segmentação (1 > 2 > 3 > 4)** | **Input:** imagens de teste ou patches de validação.<br>**Feedback:** mapas segmentados e métricas de desempenho.<br>**Plano:** carregar dataset → selecionar modelo → executar inferência → analisar métricas.<br>**Recomendação:** disponibilizar métricas detalhadas e comparações entre modelos. |
| **1. Carregar conjunto de imagens de teste (1.1 > 1.2)** | **Plano:** enviar dataset de validação.<br>Problema: dataset pode conter formatos inconsistentes.<br>Recomendação: validar automaticamente formatos e tamanho. |
| **1.1 Selecionar patches de validação** | **Problema:** seleção manual pode ser demorada.<br>Recomendação: permitir upload em lote. |
| **1.2 Confirmar upload das imagens** | **Feedback:** mostrar lista de arquivos enviados.<br>Recomendação: permitir remoção de arquivos antes do processamento. |
| **2. Selecionar arquitetura de modelo (2.1 > 2.2)** | **Plano:** escolher arquitetura para teste.<br>Problema: dificuldade em comparar arquiteturas rapidamente.<br>Recomendação: mostrar métricas resumidas ao lado da seleção. |
| **2.1 Escolher modelo (V0, V1 ou V2)** | **Problema:** diferenças técnicas pouco claras.<br>Recomendação: incluir descrição da arquitetura e dataset usado. |
| **2.2 Ver métricas e arquitetura do modelo** | **Problema:** interpretação das métricas.<br>Recomendação: explicar métricas como mIoU e IoU por classe. |
| **3. Executar segmentação automática** | **Ação:** rodar segmentação pixel a pixel.<br>Problema: processamento pode ser demorado.<br>Recomendação: permitir execução em batch ou GPU. |
| **4. Analisar resultados (4.1 / 4.2)** | **Plano:** avaliar resultados quantitativos e qualitativos.<br>Problema: interpretação visual difícil em classes raras.<br>Recomendação: destacar classes minoritárias. |
| **4.1 Comparar métricas (mIoU, IoU por classe)** | **Problema:** comparação manual entre experimentos.<br>Recomendação: gráfico comparativo automático. |
| **4.2 Avaliar qualidade visual das bordas** | **Feedback:** visualizar refinamento das bordas.<br>Recomendação: permitir zoom em regiões específicas. |

---

## **HTA 3 — Felipe Antunes (Consultor Ambiental)**

<img width="1262" height="430" alt="image" src="https://github.com/user-attachments/assets/77bc6fd3-504a-4602-a020-473eaebcb463" />

| Objetivos / Operações | Problemas e Recomendações |
|----------------------|---------------------------|
| **0. Gerar dados de cobertura vegetal para relatórios ambientais (1 > 2 > 3 > 4 > 5)** | **Input:** imagens da área de análise (ex.: ortofotos ou recortes de satélite). <br> **Feedback:** mapa segmentado e estatísticas por classe (vegetação, solo exposto, água etc.). <br> **Plano:** acessar sistema → carregar imagens → executar segmentação → analisar resultados → exportar dados para relatório. |
| **1. Acessar o sistema (1.1 > 1.2)** | **Problema:** login demorado ou falha de autenticação. <br> **Recomendação:** autenticação simplificada (login rápido ou integração com conta corporativa). |
| **1.1 Inserir credenciais** | Usuário digita login e senha ou usa autenticação integrada. |
| **1.2 Visualizar histórico de análises** | Acesso ao histórico/timeline de processamentos anteriores. |
| **2. Carregar imagens (2.1 > 2.2)** | **Problema:** arquivos grandes podem atrasar upload. <br> **Recomendação:** compressão automática e barra de progresso. |
| **2.1 Selecionar imagem** | Escolha da área de interesse a partir do computador ou repositório. |
| **2.2 Confirmar upload** | Pré-visualização da imagem e confirmação da área enviada. |
| **3. Executar segmentação** | **Problema:** usuários podem não entender parâmetros técnicos. <br> **Recomendação:** botão único de execução com configurações padrão otimizadas. |
| **4. Obter resultados (4.1 > 4.2 > 4.3)** | **Feedback:** visualização clara dos resultados para análise rápida. |
| **4.1 Visualizar mapa segmentado** | Interpretação espacial das classes detectadas na imagem. |
| **4.2 Copiar estatísticas** | Percentuais de cobertura vegetal e outras classes. |
| **4.3 Inserir dados no relatório** | Exportação para planilha ou relatório técnico. |
| **5. Exportar resultados (5.1 > 5.2)** | **Recomendação:** formatos compatíveis com relatórios ambientais. |
| **5.1 Exportar mapa** | Download do mapa segmentado (PNG, GeoTIFF). |
| **5.2 Exportar estatísticas** | Download das estatísticas em CSV ou planilha. |

---
## HTA 4 — Cláudia Torres (Gestora Pública)

<img width="1110" height="416" alt="image" src="https://github.com/user-attachments/assets/81675e2f-5b26-4567-bd8b-eabd3457ffb8" />

| Objetivos / Operações | Problemas e Recomendações |
|---|---|
| **0. Avaliar dados de uso do solo para planejamento urbano (1 > 2 > 3 > 4)** | **Input:** mapas temáticos e estatísticas geradas pelo sistema.<br>**Feedback:** visualizações claras e relatórios resumidos para análise.<br>**Plano:** acessar o dashboard → visualizar mapas → analisar estatísticas → apresentar resultados.<br>**Recomendação:** priorizar visualizações simples, intuitivas e de fácil interpretação. |
| **1. Acessar dashboard do sistema (1.1 > 1.2)** | **Plano:** abrir o sistema e selecionar uma análise disponível.<br>**Problema:** dificuldade de navegação ou localização das análises.<br>**Recomendação:** utilizar menu simples e organização clara das análises. |
| **1.1 Abrir plataforma GeoSegment** | **Problema:** acesso lento ou instável dependendo da conexão.<br>**Recomendação:** otimizar carregamento da plataforma no navegador. |
| **1.2 Selecionar análise disponível** | **Problema:** múltiplas análises podem gerar confusão para o usuário.<br>**Recomendação:** destacar análises recentes ou mais relevantes. |
| **2. Visualizar mapas temáticos (2.1 > 2.2)** | **Plano:** observar a distribuição espacial das classes no mapa.<br>**Problema:** excesso de camadas ou informações visuais.<br>**Recomendação:** permitir ativar ou desativar camadas do mapa. |
| **2.1 Visualizar mapa segmentado** | **Feedback:** mapa colorido facilita a compreensão das classes de uso do solo.<br>**Recomendação:** incluir legenda clara e padronizada para cada classe. |
| **2.2 Comparar áreas urbanas e vegetação** | **Problema:** dificuldade em perceber mudanças ou diferenças entre áreas.<br>**Recomendação:** permitir comparação temporal ou visualização lado a lado. |
| **3. Analisar estatísticas (3.1 > 3.2)** | **Plano:** examinar os dados quantitativos gerados pela segmentação.<br>**Problema:** grande volume de números pode dificultar a interpretação.<br>**Recomendação:** utilizar gráficos e indicadores visuais para facilitar a análise. |
| **3.1 Analisar estatísticas por histórico** | **Feedback:** visualização da evolução dos dados ao longo do tempo.<br>**Recomendação:** permitir filtros por período ou comparação entre análises. |
| **3.2 Analisar estatísticas por classe** | **Feedback:** percentuais de cada classe de uso do solo (vegetação, urbano, água etc.).<br>**Recomendação:** apresentar gráficos de barras ou pizza para facilitar a interpretação. |
| **4. Apresentar resultados** | **Plano:** utilizar os dados em reuniões ou decisões estratégicas.<br>**Problema:** comunicação técnica pode ser difícil para alguns usuários.<br>**Recomendação:** gerar relatórios visuais resumidos e de fácil entendimento. |

---
## HTA 5 — Sr. Benedito (Proprietário Rural)

<img width="923" height="371" alt="image" src="https://github.com/user-attachments/assets/11f03b07-4cfa-45f8-b012-fc998215ae0d" />

| Objetivos / Operações | Problemas e Recomendações |
|---|---|
| **0. Verificar classificação da propriedade no mapa (1 > 2 > 3)** | **Input:** mapa segmentado da propriedade.<br>**Feedback:** visualização clara da área agrícola.<br>**Plano:** acessar mapa → localizar propriedade → verificar classificação.<br>**Recomendação:** interface simples e fácil de entender. |
| **1. Acessar visualização do mapa (1.1 > 1.2)** | **Plano:** abrir sistema e encontrar propriedade.<br>**Problema:** dificuldade com tecnologia.<br>**Recomendação:** interface simplificada e navegação intuitiva. |
| **1.1 Abrir sistema com ajuda do neto** | **Problema:** pouca familiaridade com tecnologia.<br>**Recomendação:** tutorial simples ou assistência inicial. |
| **1.2 Localizar propriedade no mapa** | **Problema:** dificuldade em encontrar a área correta.<br>**Recomendação:** busca por coordenadas, endereço ou nome da propriedade. |
| **2. Ver classificação da área (2.1 > 2.2)** | **Plano:** observar a classificação da terra apresentada no mapa.<br>**Problema:** cores ou termos técnicos difíceis de entender.<br>**Recomendação:** legenda clara e linguagem simples. |
| **2.1 Identificar área agrícola** | **Problema:** confusão entre classes similares (ex.: vegetação esparsa e agricultura).<br>**Recomendação:** destacar visualmente a área da propriedade. |
| **2.2 Comparar com situação real** | **Problema:** dúvidas sobre a precisão da classificação automática.<br>**Recomendação:** apresentar nível de confiança da classificação. |
| **3. Confirmar resultado (3.1 > 3.2)** | **Plano:** verificar se a classificação apresentada corresponde à realidade da propriedade.<br>**Problema:** insegurança quanto à decisão ou interpretação dos dados.<br>**Recomendação:** oferecer suporte técnico ou explicação adicional sobre o resultado. |
| **3.1 Verificar limites da propriedade** | **Problema:** limites podem não estar claros no mapa.<br>**Recomendação:** destacar contorno da propriedade com borda visível. |
| **3.2 Confirmar classificação da área** | **Feedback:** confirmação visual da classe atribuída à propriedade.<br>**Recomendação:** permitir visualizar detalhes da classificação e possíveis ajustes. |
