# Análise de Concorrência

---

# 1. Identificação dos Competidores e Público-Alvo

## Público-Alvo
Especialistas ambientais, analistas do ICMBio e pesquisadores que necessitam de mapeamento de uso e cobertura do solo em áreas de conservação, como a APA de Petrópolis.

---

## Competidores Tradicionais (Desktop GIS)
- QGIS
- ArcGIS Pro

Características gerais:
- Ferramentas generalistas de geoprocessamento
- Alto nível de controle técnico
- Processamento majoritariamente local

---

## Competidores em Nuvem (SaaS / AIaaS)

- **MapBiomas** – Plataforma web para visualização e análise anual de uso e cobertura do solo.
- **Brazil Data Cube / TerraCollect** – Plataforma web para coleta de amostras e análise de séries temporais.
- **ArcGIS Living Atlas (Esri)** – Base de dados e serviços geoespaciais integrados ao ecossistema ArcGIS Online.

Características gerais:
- Processamento remoto
- Acesso via navegador
- Foco em visualização e análise temática
- Dependência de infraestrutura em nuvem

---

# 2. Análise de Características e Funcionalidades

## GeoSegment – Pontos Fortes
- Segmentação automática via Deep Learning
- Identificação de detalhes finos (edificações, fragmentos de vegetação)
- Alta resolução espacial
- Aplicação leve com fluxo encapsulado
- Modelo AIaaS (processamento remoto)
- Interface focada em tarefa única

---

## Competidores Tradicionais – Pontos Fracos
- Instalação local obrigatória
- Dependência de hardware potente
- Curva de aprendizado elevada
- Alta complexidade operacional
- Necessidade de parametrização manual

---

## Competidores AI SaaS – Limitações

### MapBiomas
- Interface focada em visualização, não em segmentação customizada
- Baixa possibilidade de ajuste fino pelo usuário
- Dados predefinidos (usuário não treina modelo)

### Brazil Data Cube / TerraCollect
- Interface técnica
- Exige entendimento de séries temporais
- Processo de coleta e classificação não totalmente automatizado

### ArcGIS Living Atlas
- Integração robusta com ecossistema Esri
- Dependência de assinatura/licenciamento
- Interface densa e orientada a múltiplos serviços

---

# 3. Avaliação da Experiência do Usuário (UX) e Interface (IHC)

---

# Área para Imagens das Interfaces

## QGIS
<img width="1654" height="771" alt="qgis" src="https://github.com/user-attachments/assets/b797921d-3fba-4e5d-acc2-aac9d395ff93" />

*Figura X – Interface principal do QGIS com múltiplos painéis e barras de ferramentas.*

---

## ArcGIS Pro
<img width="648" height="414" alt="arcgis" src="https://github.com/user-attachments/assets/9bc4210e-78d8-4406-a034-c5deb100a8c1" />

*Figura Y – Interface do ArcGIS Pro com Ribbon e painel de camadas.*

---

## MapBiomas
![INSERIR IMAGEM DO MAPBIOMAS AQUI]

*Figura Z – Dashboard web do MapBiomas para visualização temática.*

---

## Brazil Data Cube / TerraCollect
![INSERIR IMAGEM DO BDC AQUI]

*Figura W – Portal web do Brazil Data Cube.*

---

## GeoSegment
![INSERIR IMAGEM DO GEOSEGMENT AQUI]

*Figura K – Interface simplificada e orientada à tarefa do GeoSegment.*

---

# 3.1 Comparação de Estilo de Interface

| Ferramenta | Tipo | Estilo de Interface | Complexidade Visual | Curva de Aprendizado |
|------------|------|--------------------|--------------------|----------------------|
| QGIS | Desktop | WIMP tradicional | Alta | Alta |
| ArcGIS Pro | Desktop | Ribbon + múltiplos painéis | Alta | Alta |
| MapBiomas | Web SaaS | Dashboard temático | Média | Média |
| Brazil Data Cube | Web SaaS | Interface técnica | Média-Alta | Média-Alta |
| GeoSegment | Web AIaaS | Minimalista orientada à tarefa | Baixa | Baixa |

---

# 3.2 Modelo de Interação

## QGIS / ArcGIS
- Modelo exploratório
- Múltiplas camadas (layers)
- Parametrização manual
- Alto grau de liberdade técnica

Impacto:
- Alta carga cognitiva
- Necessidade de formação técnica
- Maior probabilidade de erro operacional

---

## MapBiomas / BDC / Living Atlas
- Modelo de exploração de dados
- Visualização temática
- Processamento majoritariamente invisível ao usuário
- Interação baseada em filtros e consultas

Impacto:
- Média carga cognitiva
- Menor controle sobre modelos
- Usuário atua mais como analista interpretativo

---

## GeoSegment
- Modelo orientado à tarefa
- Fluxo linear:
  1. Selecionar área
  2. Executar segmentação
  3. Visualizar resultado
  4. Exportar dados

Impacto:
- Baixa carga cognitiva
- Redução de decisões técnicas
- Automação do processamento
- Foco na tomada de decisão

---

# 3.3 Comparação de Fluxo de Tarefas

| Etapa | QGIS/ArcGIS | AI SaaS (MapBiomas/BDC) | GeoSegment |
|-------|-------------|-------------------------|------------|
| Instalação | Necessária | Não | Não |
| Configuração técnica | Alta | Média | Baixa |
| Execução de modelo | Manual | Automática (predefinida) | Automática personalizada |
| Exportação | Manual | Disponível | Simplificada |
| Feedback visual | Variável | Imediato | Imediato |

---

# 3.4 Carga Cognitiva

## Alta – QGIS / ArcGIS
- Múltiplos menus
- Parâmetros técnicos
- Interface densa
- Exposição simultânea de muitas funcionalidades

## Média – AI SaaS
- Menos parâmetros técnicos
- Interface mais limpa
- Dependência de entendimento conceitual

## Baixa – GeoSegment
- Processo automatizado
- Interface simplificada
- Exposição mínima de opções técnicas
- Redução de esforço mental

---

# 3.5 Controle vs Automação

| Ferramenta | Nível de Controle do Usuário | Nível de Automação |
|------------|-----------------------------|--------------------|
| QGIS | Muito alto | Baixo |
| ArcGIS | Alto | Médio |
| MapBiomas | Baixo | Alto |
| Brazil Data Cube | Médio | Médio |
| GeoSegment | Médio (controlado) | Alto |

O GeoSegment posiciona-se como um modelo intermediário, equilibrando automação com controle suficiente para aplicações especializadas.

---

# 4. Tendências de Mercado

- Migração de SIG desktop para plataformas web
- Crescimento do modelo AIaaS
- Integração entre aprendizado de máquina e geoprocessamento
- Redução da complexidade da interface
- Foco em especialização ao invés de generalização

O GeoSegment está alinhado a essas tendências ao oferecer segmentação como serviço especializado via navegador.

---

# 5. Recomendações Estratégicas

## Diferencial Competitivo
- Especialização em alta resolução
- Segmentação automática simplificada
- Interface minimalista orientada à tarefa
- Redução de barreiras técnicas

## Pontos de Melhoria
- Expansão do dataset para maior generalização
- Implementação de histórico de inferências
- Inclusão de métricas detalhadas:
  - Matriz de confusão
  - IoU por classe
  - Boundary IoU
- Ferramenta de comparação visual com ground truth
- Controle opcional de parâmetros avançados (modo especialista)

O GeoSegment propõe um equilíbrio entre automação e especialização, com foco em usabilidade, redução da complexidade e alinhamento às tendências contemporâneas de Inteligência Artificial como Serviço.
