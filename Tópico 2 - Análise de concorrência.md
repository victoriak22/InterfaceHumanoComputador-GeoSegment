# Análise de Concorrência – Plataformas de Geoprocessamento e Segmentação

---

# 1. Identificação dos Competidores e Público-Alvo

## Público-Alvo

Especialistas ambientais, analistas do ICMBio, gestores de unidades de conservação e pesquisadores que necessitam de mapeamento de uso e cobertura do solo, especialmente em áreas protegidas como a APA de Petrópolis.

Esses usuários normalmente apresentam:

- Conhecimento técnico em geoprocessamento ou sensoriamento remoto  
- Necessidade de precisão cartográfica  
- Demanda por dados confiáveis para relatórios e tomada de decisão  
- Limitação de tempo para tarefas altamente operacionais  

---

# 2. Categorias de Competidores

## 2.1 Ferramentas Desktop (SIG Tradicionais)

- **QGIS**
- **ArcGIS Pro**

### Características Gerais

- Ferramentas generalistas de geoprocessamento
- Grande flexibilidade analítica
- Alto nível de controle manual
- Processamento predominantemente local
- Estrutura baseada em múltiplas camadas (layers)

Essas ferramentas são consolidadas no mercado e amplamente utilizadas em ambientes institucionais e acadêmicos.

---

## 2.2 Plataformas Web (SaaS / AIaaS)

- **MapBiomas**
- **Brazil Data Cube / TerraCollect**
- **ArcGIS Living Atlas (Esri)**

### Características Gerais

- Processamento remoto
- Acesso via navegador
- Foco em visualização temática e análise exploratória
- Dependência de infraestrutura em nuvem
- Menor necessidade de configuração local

Essas plataformas seguem a tendência de migração para serviços baseados em nuvem.

---

# 3. Análise de UX (Experiência do Usuário) e Interface

## QGIS

<img width="1654" height="771" alt="qgis" src="https://github.com/user-attachments/assets/b797921d-3fba-4e5d-acc2-aac9d395ff93" />

*Figura 1 – Interface principal do QGIS com múltiplos painéis e barras de ferramentas.*

---

- Interface baseada no modelo WIMP (Windows, Icons, Menus, Pointer)
- Grande número de painéis e barras de ferramentas
- Forte personalização
- Alta densidade informacional

### Pontos Positivos
- Flexibilidade total
- Alto controle sobre dados e processos
- Ecossistema de plugins

### Pontos Críticos
- Pode ser visualmente sobrecarregado
- Exige familiaridade prévia
- Curva de aprendizado elevada

**Intuitividade:**  
Baixa para iniciantes; moderada para usuários experientes.

---

## ArcGIS Pro
<img width="648" height="414" alt="arcgis" src="https://github.com/user-attachments/assets/9bc4210e-78d8-4406-a034-c5deb100a8c1" />

*Figura 2 – Interface do ArcGIS Pro com Ribbon e painel de camadas.*

---

- Interface com Ribbon (inspirada no pacote Microsoft Office)
- Organização modular por abas
- Integração com ecossistema ArcGIS

### Pontos Positivos
- Estrutura visual organizada
- Padrão corporativo consistente
- Integração com serviços online

### Pontos Críticos
- Complexidade técnica
- Dependência de licenciamento
- Alto número de ferramentas simultâneas

**Intuitividade:**  
Moderada. A organização é clara, mas a quantidade de recursos aumenta a carga cognitiva.

---

## MapBiomas
![mapbiomas](https://github.com/user-attachments/assets/9fd5e2f7-3e83-486b-b1b2-0dbc4b11c3c0)

*Figura 3 – Dashboard web do MapBiomas para visualização temática.*

---

- Dashboard web
- Foco em visualização temática
- Navegação baseada em filtros e seleção temporal

### Pontos Positivos
- Interface limpa
- Fácil exploração de séries históricas
- Curva de aprendizado reduzida

### Pontos Críticos
- Pouca customização
- Usuário não controla o modelo de classificação
- Foco em consulta, não em processamento personalizado

**Intuitividade:**  
Alta para exploração; limitada para análises avançadas.

---

## Brazil Data Cube / TerraCollect
![info-cube-bdc](https://github.com/user-attachments/assets/a6ab5504-d5a5-4f88-9d34-bf0362f8aac8)

*Figura 4 – Portal web do Brazil Data Cube.*

---

- Interface técnica voltada à coleta de amostras
- Foco em séries temporais
- Estrutura orientada a especialistas

### Pontos Positivos
- Adequado para pesquisadores
- Estrutura metodologicamente robusta
- Integração com dados orbitais

### Pontos Críticos
- Interface menos amigável
- Requer conhecimento prévio em classificação
- Processo menos automatizado

**Intuitividade:**  
Média-baixa. Voltada a usuários técnicos.

---

## ArcGIS Living Atlas

- Plataforma integrada ao ArcGIS Online
- Catálogo de dados e serviços geoespaciais
- Interface baseada em navegação por camadas

### Pontos Positivos
- Grande volume de dados prontos
- Integração fluida com outras ferramentas Esri
- Visualização eficiente

### Pontos Críticos
- Dependência de assinatura
- Ecossistema fechado
- Interface densa para novos usuários

**Intuitividade:**  
Moderada, especialmente para usuários já inseridos no ecossistema Esri.

---

# 4. Modelos de Interação

## 4.1 Modelo Exploratórico (Desktop SIG)

- Manipulação manual de camadas
- Configuração detalhada de parâmetros
- Alto grau de liberdade

**Impacto:**
- Alta carga cognitiva
- Maior controle
- Maior risco de erro operacional

---

## 4.2 Modelo de Exploração Temática (SaaS)

- Interface baseada em filtros
- Processamento invisível ao usuário
- Ênfase na visualização

**Impacto:**
- Redução da complexidade técnica
- Menor controle sobre modelos
- Experiência mais guiada

---

# 5. Comparação de Fluxo de Tarefas

| Etapa | QGIS/ArcGIS | MapBiomas | BDC | Living Atlas |
|-------|-------------|------------|-----|--------------|
| Instalação | Necessária | Não | Não | Não |
| Configuração técnica | Alta | Baixa | Média | Baixa |
| Processamento | Manual | Pré-definido | Semi-manual | Pré-configurado |
| Exportação | Manual | Disponível | Disponível | Integrada |
| Feedback visual | Variável | Imediato | Moderado | Imediato |

---

# 6. Carga Cognitiva

## Alta
- QGIS
- ArcGIS Pro

Devido à multiplicidade de ferramentas e decisões técnicas.

## Média
- Brazil Data Cube
- ArcGIS Living Atlas

Exigem entendimento conceitual, mas reduzem parametrização manual.

## Baixa
- MapBiomas

Foco em visualização e consulta simplificada.

---

# 7. Pontos Positivos Extraídos da Concorrência

- Organização modular (ArcGIS Pro)
- Simplicidade de acesso via navegador (MapBiomas)
- Robustez metodológica (BDC)
- Integração de dados em larga escala (Living Atlas)

---

# 8. Tendências Observadas

- Migração do processamento local para nuvem
- Redução da complexidade de interface
- Automação crescente por meio de IA
- Especialização de ferramentas
- Interfaces mais orientadas à tarefa
- Diminuição da necessidade de configuração manual

---

# 9. Síntese da Análise

O mercado de geoprocessamento apresenta dois polos principais:

1. **Ferramentas altamente flexíveis e complexas**, voltadas a especialistas.
2. **Plataformas web simplificadas**, focadas em visualização e acesso rápido à informação.

A principal diferença competitiva entre essas soluções está no equilíbrio entre:

- Controle técnico  
- Nível de automação  
- Intuitividade da interface  
- Carga cognitiva exigida do usuário  

Ferramentas desktop privilegiam profundidade analítica, enquanto plataformas SaaS priorizam acessibilidade e redução de barreiras técnicas.

Essa dinâmica revela uma tendência clara de especialização e simplificação progressiva da experiência do usuário no setor de geotecnologias.
