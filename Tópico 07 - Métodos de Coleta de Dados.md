# Tópico 07 - Métodos de Coleta de Dados

Este documento descreve os **instrumentos de coleta de dados** utilizados no projeto *GeoSegment*, abrangendo tanto técnicas quantitativas quanto qualitativas. Cada método é apresentado com seu respectivo responsável, definição, aplicabilidade, vantagens, limitações e forma de uso no contexto do projeto.

## Sumário

- [Questionário](#questionario)
- [Entrevista (semiestruturada)](#entrevista-semiestruturada)
- [Classificação de Cartões (Card Sorting)](#card-sorting)
- [Observação Participante](#observacao-participante)
- [Grupo de Foco (Focus Group)](#grupo-de-foco)

---

<a id="questionario"></a>

## Questionário

**Responsável:** Victor Caldeira Iak - 22.122.057-7  

**Link do instrumento:**  
https://form.typeform.com/to/hVWylPj9

---

<a id="entrevista-semiestruturada"></a>

## Entrevista (semiestruturada)

**Responsável:** Lucas Rebouças Silva – 22.122.048-6  

### Definição

A entrevista semiestruturada consiste em uma técnica qualitativa baseada em um roteiro flexível de perguntas abertas, permitindo ao entrevistador adaptar a condução conforme o perfil do participante e aprofundar aspectos relevantes ao longo da interação.

### Aplicabilidade

É indicada quando se busca compreender em profundidade:

- motivações e percepções dos usuários  
- contexto de trabalho  
- vocabulário adotado no domínio de aplicação  

No contexto do *GeoSegment*, essa técnica complementa dados quantitativos provenientes de questionários e contribui para a validação de hipóteses relacionadas a fluxos de trabalho, dificuldades e expectativas dos usuários.

### Vantagens

- Permite o esclarecimento imediato de respostas ambíguas  
- Favorece a identificação de necessidades implícitas  
- Produz narrativas relevantes para a construção de personas e cenários (em alinhamento com os Tópicos 03 e 04)  

### Limitações

- Envolve amostras reduzidas e maior tempo por participante  
- Depende da habilidade do entrevistador e da qualidade do recrutamento  
- Exige registro fiel e análise qualitativa estruturada  

### Aplicação no contexto do projeto

No *GeoSegment*, a entrevista é direcionada a profissionais que atuam com análise de imagens aéreas, segmentação e apoio à decisão territorial. São abordados aspectos como:

- fluxo de trabalho (upload, processamento e análise)  
- escolha e interpretação de modelos e métricas  
- uso de dashboards e visualizações  
- comparação temporal  
- histórico de processamentos  

O objetivo é compreender como a ferramenta pode se integrar às práticas atualmente adotadas (ex.: QGIS, relatórios técnicos) e quais fatores influenciam a confiança nos resultados.

### Roteiro de entrevista

O roteiro foi estruturado em blocos temáticos, permitindo adaptação conforme o perfil do participante (analista, pesquisador ou gestor), mantendo consistência na coleta de dados.

#### 1. Perfil do usuário (demografia e experiência)

- Qual sua formação e há quanto tempo atua com análise ambiental ou geoespacial?
- Em qual instituição ou tipo de projeto você trabalha atualmente?
- Com que frequência lida com mapas de uso e cobertura do solo ou fiscalização territorial?

#### 2. Uso de tecnologia (habilidades e ferramentas)

- Quais softwares ou serviços utiliza com maior frequência (GIS, planilhas, nuvem, notebooks)?
- Como avalia seu nível de conhecimento em geoprocessamento e em modelos estatísticos ou de inteligência artificial?
- Prefere trabalhar em ambiente web, desktop ou uma combinação de ambos?

#### 3. Tarefas (fluxos e objetivos)

- Descreva um fluxo típico de trabalho envolvendo análise de imagens aéreas.
- Com que frequência realiza comparações temporais ou gera relatórios quantitativos?
- Quais etapas são necessárias para transformar dados brutos em uma análise utilizável?

#### 4. Dificuldades (gargalos e limitações)

- Quais são os principais obstáculos enfrentados no processo atual?
- Existem etapas que exigem retrabalho frequente?
- Em que momentos as ferramentas utilizadas deixam de atender às necessidades?

#### 5. Necessidades (melhorias desejadas)

- Que tipo de informação gostaria de visualizar de forma integrada?
- O que aumentaria sua confiança em resultados automatizados?
- Que nível de rastreabilidade dos processamentos considera adequado?

#### 6. Sistema ideal (expectativas futuras)

- Se pudesse projetar uma interface ideal, quais elementos seriam indispensáveis?
- Como prefere exportar ou compartilhar resultados?
- O que caracterizaria o sucesso de uma ferramenta como o *GeoSegment* no seu contexto de trabalho?

---

<a id="card-sorting"></a>

## Classificação de Cartões (Card Sorting)

**Responsável:** Deise Adriana Silva Araújo – 22.222.024-6  

### Definição

A classificação de cartões (*card sorting*) é uma técnica utilizada para compreender como os usuários organizam informações de acordo com seu modelo mental, por meio do agrupamento de itens em categorias significativas.

A técnica pode ser aplicada em dois formatos:

- **Aberto:** os participantes criam e nomeiam as categorias  
- **Fechado:** as categorias são previamente definidas  

### Aplicabilidade

É recomendada sua aplicação em fases iniciais de definição da arquitetura da informação, especialmente para:

- organização da navegação  
- definição da hierarquia de funcionalidades  
- padronização de nomenclaturas  

No *GeoSegment*, mostra-se particularmente relevante para estruturar a interface principal e alinhar a terminologia ao vocabulário de analistas ambientais.

### Vantagens

- Evidencia o vocabulário natural dos usuários  
- Reduz o uso de terminologia técnica inadequada  
- Apresenta baixo custo e possibilidade de aplicação remota  
- Produz resultados diretamente aplicáveis ao design de interface  
- Permite a comparação entre diferentes perfis de usuários  

### Limitações

- Não representa o comportamento real de uso  
- Perde confiabilidade com grande volume de cartões  
- Requer análise estruturada (ex.: matriz de similaridade, dendrogramas)  

### Aplicação no contexto do projeto

Serão elaborados entre 20 e 30 cartões contendo funcionalidades e informações do sistema, tais como envio de imagem, visualização de mapa segmentado, proporção por classe, histórico de processamentos, comparação temporal, exportação de dados, entre outros.

A técnica será aplicada no formato aberto com analistas ambientais e pesquisadores. Os agrupamentos mais recorrentes subsidiarão a definição da navegação e da hierarquia visual da interface.

### Instrumento

Ferramenta sugerida: Optimal Workshop (OptimalSort) ou cartões físicos em sessões presenciais.

---

<a id="observacao-participante"></a>

## Observação Participante

**Responsável:** Gustavo Dias Vicentin – 22.123.061-8  

### Definição

A observação participante consiste no acompanhamento do usuário em seu contexto real de trabalho, permitindo a análise de comportamentos espontâneos. O observador pode interagir de forma controlada, sem interferir na execução das atividades.

### Aplicabilidade

É indicada quando há potencial divergência entre o comportamento declarado e o comportamento efetivamente realizado.

No contexto do *GeoSegment*, essa técnica permite compreender:

- fluxos reais de trabalho  
- uso simultâneo de ferramentas  
- estratégias informais e adaptações não padronizadas  
- pontos críticos do processo  

### Vantagens

- Captura comportamentos não verbalizados  
- Evidencia o ambiente real de trabalho  
- Gera insumos para modelagem de fluxos e cenários  
- Permite compreender decisões em tempo real  

### Limitações

- Possível alteração de comportamento devido à observação  
- Exige acesso presencial ou remoto ao ambiente do usuário  
- Demanda esforço significativo de registro e análise  
- Dependência da disponibilidade dos participantes  

### Aplicação no contexto do projeto

Serão realizadas, no mínimo, duas sessões de observação com analistas que atuam no processamento de imagens aéreas. Serão analisados aspectos como:

- origem e organização das imagens  
- sequência de ferramentas utilizadas  
- critérios de validação dos resultados  
- formas de registro e comunicação  
- momento da tomada de decisão  

O registro será realizado por meio de anotações estruturadas e, quando autorizado, gravação de tela.

### Roteiro de observação

| Momento | O que observar |
|--------|--------------|
| Início da tarefa | Origem e organização das imagens |
| Processamento | Ferramentas utilizadas e sequência |
| Análise do resultado | Estratégias de validação |
| Registro | Formas de documentação |
| Compartilhamento | Destinatários e formatos |
| Interrupções | Fatores que impactam o fluxo |

---

<a id="grupo-de-foco"></a>

## Grupo de Foco (Focus Group)

**Responsável:** Vinicius Saidi Soares – 22.122.064-3  

### Definição

O grupo de foco consiste em uma sessão mediada com múltiplos participantes, na qual são discutidos temas previamente definidos. A interação entre os participantes possibilita a identificação de convergências, divergências e prioridades coletivas.

### Aplicabilidade

É indicado quando se busca integrar diferentes perspectivas sobre um mesmo conjunto de funcionalidades.

No *GeoSegment*, será utilizado para alinhar expectativas entre analistas ambientais, pesquisadores e gestores territoriais.

### Vantagens

- Produz grande volume de informações em curto período  
- Evidencia prioridades coletivas  
- Permite validação colaborativa de soluções  
- Favorece alinhamento conceitual entre perfis distintos  

### Limitações

- Risco de influência entre participantes (*groupthink*)  
- Complexidade logística  
- Possível inibição em contextos hierárquicos  
- Dependência da qualidade da moderação  

### Aplicação no contexto do projeto

Será conduzida uma sessão com duração entre 60 e 90 minutos, estruturada em três etapas: diagnóstico do fluxo atual, apresentação da ferramenta e priorização de funcionalidades. A dinâmica poderá ser apoiada por ferramentas colaborativas.

### Questões-guia por bloco

**Bloco 1 – Diagnóstico**
- Como ocorre o fluxo atual de trabalho, desde a obtenção das imagens até a geração de resultados?
- Quais são os principais gargalos identificados nesse processo?
- Quem são os principais usuários dos resultados gerados e em quais formatos eles são consumidos?

**Bloco 2 – Reação**
- O que chamou atenção, de forma positiva ou negativa, na utilização da ferramenta?
- O que seria necessário para aumentar a confiança nos resultados automatizados?
- Quais informações relevantes não estão atualmente disponíveis?

**Bloco 3 – Priorização**
- Entre as funcionalidades propostas, quais devem ser priorizadas?
- Quais condições mínimas são necessárias para adoção da ferramenta no contexto de trabalho?
