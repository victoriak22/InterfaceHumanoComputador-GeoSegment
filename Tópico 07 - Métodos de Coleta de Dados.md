# Tópico 07 - Métodos de Coleta de Dados

Este documento descreve os **dois instrumentos** de coleta de dados utilizados no projeto GeoSegment: questionário online e entrevista semiestruturada. Cada técnica tem um responsável na equipe.

## Sumário

- [Questionário](#questionario)
- [Entrevista (semiestruturada)](#entrevista-semiestruturada)
- [Classificação de Cartões (Card Sorting)](#card-sorting)
- [Observação Participante](#observacao-participante)
- [Grupo de Foco (Focus Group)](#grupo-de-foco)

---

<a id="questionario"></a>

## Questionário

**Responsável:** Victor Caldeira Iak - 22.122.057-7.

**Link do instrumento:** [https://form.typeform.com/to/hVWylPj9](https://form.typeform.com/to/hVWylPj9)

---

<a id="entrevista-semiestruturada"></a>

## Entrevista (semiestruturada)

**Responsável:** Lucas Rebouças Silva – 22.122.048-6.

### Definição breve

Conversa guiada por um roteiro de temas e perguntas abertas, com liberdade para aprofundar respostas. O entrevistador adapta a ordem e o nível de detalhe conforme o perfil do participante.

### Quando utilizar

Quando se buscam motivações, contexto de trabalho e vocabulário do usuário em profundidade. Complementa dados quantitativos (como um questionário) e ajuda a validar hipóteses sobre fluxos e dores na análise de imagens e decisão territorial.

### Vantagens

- Permite esclarecer respostas ambíguas na hora.
- Revela necessidades tácitas que o participante não formulou por escrito.
- Gera narrativas úteis para personas e cenários (alinhado ao [Tópico 03](Tópico%2003%20-%20Usuários.md) e ao [Tópico 04](Tópico%2004%20-%20Cenário%20de%20Análise%20de%20Problemas.md)).

### Limitações

- Amostra pequena e tempo maior por sessão.
- Resultados dependem da condução da entrevista e do recrutamento.
- Análise qualitativa exige registro fiel (gravação com consentimento ou anotações estruturadas).

### Como aplicar no contexto do projeto

No **GeoSegment**, a entrevista foca quem trabalha com imagens aéreas, segmentação e apoio à decisão: upload e processamento, escolha de modelo, leitura de métricas, dashboards, comparação temporal e histórico de processamentos. O objetivo é mapear expectativas de interface, confiança nos resultados e integração com o fluxo atual (ex.: QGIS, relatórios).

### Roteiro de entrevista

O roteiro foi estruturado em blocos temáticos, permitindo adaptação conforme o perfil do participante (analista, pesquisador ou gestor), mantendo, contudo, consistência na coleta dos dados.

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
- O que caracterizaria o sucesso de uma ferramenta como o GeoSegment no seu contexto de trabalho?

---

<a id="card-sorting"></a>

## Classificação de Cartões (Card Sorting)

**Responsável:** Deise Adriana Silva Araújo – 22.222.024-6
### Definição breve

Técnica em que os participantes agrupam itens escritos em cartões (físicos ou digitais) em categorias que fazem sentido para eles. No modelo aberto, os próprios participantes criam e nomeiam os grupos. No modelo fechado, as categorias já existem e o participante apenas distribui os cartões. O objetivo é entender como o usuário organiza mentalmente a informação.

### Quando utilizar

Quando precisamos decidir como organizar a interface antes de prototipar, especialmente a navegação e a hierarquia das funcionalidades. No GeoSegment, faz sentido aplicar antes de definir a estrutura da tela principal: o que fica visível logo de cara, o que vai em aba separada, como nomear as classes de cobertura do solo de um jeito que o analista ambiental reconheça sem precisar de explicação.

### Vantagens

- Revela o vocabulário natural do usuário, o que evita que a interface use termos técnicos que fazem sentido para a gente mas não para quem vai usar (por exemplo, o analista pode chamar de "mapa" o que a gente chama de "máscara segmentada").
- É barato e pode ser aplicado remotamente com ferramentas como Optimal Workshop ou Maze.
- Os resultados alimentam diretamente decisões de layout, menus e agrupamentos de funcionalidade.
- Permite comparar como perfis diferentes (analista de campo, pesquisador, gestor) organizam as mesmas informações.

### Limitações

- Não captura comportamento real de uso, só preferências declaradas de organização.
- Com muitos cartões (mais de 40), o participante se perde e os agrupamentos deixam de ser confiáveis.
- A análise dos resultados exige algum esforço: é preciso montar uma matriz de similaridade ou dendrograma para consolidar os padrões que aparecem entre os participantes.

### Como aplicar no contexto do projeto

Criar entre 20 e 30 cartões com funcionalidades e informações do GeoSegment: Enviar imagem, Ver mapa segmentado, Proporção por classe, Histórico de processamentos, Comparar datas diferentes, Exportar PDF, Exportar shapefile, Legenda de cores, Confiança do modelo, Área total de vegetação, Alertas de mudança, Configurar parâmetros do modelo, entre outros. Aplicar no formato aberto com analistas do ICMBio e pesquisadores, pedindo que agrupem os cartões e nomeiem as categorias do jeito que fizer mais sentido para eles. Os agrupamentos mais frequentes viram a base da navegação e da hierarquia visual da interface.

### Instrumento

Ferramenta sugerida: Optimal Workshop (OptimalSort), gratuito para até 10 participantes, ou cartões físicos em sessão presencial com analistas do ICMBio.

---

<a id="observacao-participante"></a>

## Observação Participante

**Responsável:** Gustavo Dias Vicentin – 22.123.061-8

### Definição breve

O observador acompanha o participante durante as atividades reais de trabalho e pode interagir de forma controlada: fazer perguntas pontuais, pedir que o usuário pense em voz alta, mas sem assumir o controle da tarefa. O foco é o comportamento espontâneo em contexto real, não o que o usuário diz que faz numa entrevista.

### Quando utilizar

Quando existe risco de divergência entre o que o usuário declara e o que ele realmente faz no dia a dia. No caso do GeoSegment, isso é bem relevante: analistas ambientais provavelmente descrevem um fluxo de trabalho mais organizado do que o que acontece na prática. A observação participante serve para entender quais ferramentas abrem em paralelo com o navegador, onde o fluxo trava de verdade, que gambiarras o usuário criou por conta própria e o que ele tenta delegar para evitar.

### Vantagens

- Captura comportamentos que o próprio usuário não sabe descrever porque são automáticos ou muito habituais.
- Mostra o ambiente real de trabalho: múltiplas abas abertas, arquivos nomeados de forma improvisada, limitações de hardware, interrupções frequentes.
- Gera insumos concretos para construir fluxos de tarefa e cenários de uso, alinhado ao Tópico 04 da disciplina.
- A interação controlada do observador permite entender decisões na hora, por exemplo: "por que você abriu o QGIS agora se já tinha o resultado aqui?"

### Limitações

- O participante pode mudar o comportamento por saber que está sendo observado, o chamado efeito do observador.
- Requer deslocamento ou acesso remoto à tela do usuário via ferramentas como Teams ou Lookback.
- A análise é trabalhosa e requer registro fiel por gravação de tela ou anotações estruturadas feitas durante a sessão.
- Pode ser difícil negociar horário com analistas do ICMBio em período de trabalho.

### Como aplicar no contexto do projeto

Acompanhar ao menos duas sessões de trabalho real de analistas que processam imagens aéreas da APA de Petrópolis ou de regiões similares. Observar especificamente de onde vêm as imagens brutas e como são organizadas, quais softwares são abertos em sequência (QGIS, ArcGIS, Excel, relatórios), como o analista valida visualmente o resultado de uma segmentação, como documenta o que encontrou e em que momento a decisão de gestão territorial é tomada. Registrar por anotações estruturadas e, se houver consentimento, gravação de tela.

### Roteiro de observação (checklist de foco)

| Momento | O que observar |
|--------|--------------|
| Início da tarefa | De onde vêm as imagens? Como são nomeadas e organizadas? |
| Processamento | Quais ferramentas são abertas? Em que ordem? |
| Análise do resultado | Como valida o mapa? Compara manualmente? |
| Registro | Onde documenta os achados? Que formato usa? |
| Compartilhamento | Para quem envia? Em que formato (PDF, e-mail, sistema)? |
| Interrupções | O que faz parar o fluxo? Onde pede ajuda? |

---

<a id="grupo-de-foco"></a>

## Grupo de Foco (Focus Group)

**Responsável:** Vinicius Saidi Soares – 22.122.064-3

### Definição breve

Sessão moderada com 5 a 8 participantes de perfis complementares, conduzida por um facilitador com um roteiro de questões abertas. O diferencial em relação à entrevista individual está na dinâmica de grupo: os participantes reagem às falas uns dos outros, o que faz emergir convergências, conflitos de expectativa e prioridades coletivas que não apareceriam numa conversa a dois.

### Quando utilizar

Quando precisamos confrontar perspectivas de diferentes tipos de usuário sobre as mesmas funcionalidades. No GeoSegment, analistas de campo, pesquisadores acadêmicos e gestores ambientais têm expectativas bem diferentes sobre precisão aceitável, métricas exibidas, formato de exportação e necessidade de histórico. O grupo de foco permite levantar e priorizar requisitos de interface com todos no mesmo espaço, o que economiza tempo e já alinha expectativas entre os stakeholders.

### Vantagens

- Gera mais ideias em menos tempo do que realizar entrevistas individuais com o mesmo número de pessoas.
- A interação entre participantes provoca reações que revelam prioridades reais.
- Permite validar hipóteses de design coletivamente.
- Ajuda a alinhar o vocabulário entre perfis diferentes.

### Limitações

- Existe risco de groupthink.
- Logística difícil.
- Pode ser inadequado em contextos hierárquicos.
- Depende da qualidade da moderação.

### Como aplicar no contexto do projeto

Recrutar participantes de três perfis: analistas ambientais, pesquisadores e gestores. Conduzir sessão de 60 a 90 minutos com diagnóstico, demonstração e priorização.

### Questões-guia por bloco

**Bloco 1 – Diagnóstico**
- Como é o processo atual?
- Gargalos?
- Uso dos resultados?

**Bloco 2 – Reação**
- O que chamou atenção?
- O que falta para confiança?
- Informações ausentes?

**Bloco 3 – Priorização**
- O que priorizar?
- Condição mínima para adoção?
