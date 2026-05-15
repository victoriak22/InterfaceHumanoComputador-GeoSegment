# Planejamento de Avaliação de IHC — GeoSegment AI
Este documento apresenta o planejamento da avaliação de Interação Humano-Computador (IHC) do GeoSegment AI utilizando o framework DECIDE, proposto por Preece et al. (2002), juntamente com os princípios apresentados por Barbosa e Silva (2010).

## Introdução

O GeoSegment AI é uma plataforma web desenvolvida para realizar segmentação semântica de imagens aéreas e de satélite voltadas ao monitoramento e análise do uso do solo.<br> O sistema permite que o usuário envie imagens nos formatos JPG, PNG e TIF, escolha modelos de inteligência artificial para processamento, compare resultados ao longo do tempo e acompanhe históricos de análises já realizadas.<br>
Entre as principais funcionalidades do sistema estão:
- Home;<br>
- Upload de imagens;<br>
- Seleção de modelos de redes neurais;<br>
- Comparação temporal de áreas segmentadas;<br>
- Visualização de métricas e dashboards;<br>
- Histórico de processamentos anteriores.<br>

A avaliação será aplicada às principais telas do protótipo desenvolvido no Figma.<br>
O planejamento considera as personas e cenários de uso definidos anteriormente no projeto.

---

# D — Determinar os objetivos da avaliação

A avaliação do GeoSegment AI possui como objetivo principal analisar a usabilidade, a interação e a compreensão das funcionalidades do sistema pelos diferentes perfis de usuários envolvidos. Para isso, a avaliação busca:

- identificar problemas de usabilidade nas principais telas do sistema que possam prejudicar a experiência do usuário durante o processo de segmentação e análise de imagens;
- verificar se os usuários conseguem utilizar as funcionalidades do sistema de forma eficiente, sem dificuldades ou necessidade excessiva de suporte;
analisar se as informações apresentadas na interface, como métricas técnicas, resultados e mensagens do sistema, são claras, compreensíveis e comunicáveis;
- verificar se o fluxo de navegação e execução das tarefas é intuitivo, especialmente nas etapas de seleção de modelo, processamento da imagem e visualização dos resultados;
- avaliar se os usuários compreendem as diferenças entre os modelos de IA disponíveis e conseguem escolher a opção mais adequada para cada necessidade;
- identificar elementos da interface que possam gerar erros, dúvidas ou confusão durante o uso;
- analisar a apropriação da tecnologia pelos diferentes perfis de usuários, considerando o contexto de consultoria ambiental, pesquisa acadêmica e apoio à gestão pública;
- verificar a conformidade da interface com heurísticas de usabilidade propostas por Jakob Nielsen, principalmente em relação à visibilidade do estado do sistema, controle do usuário e clareza na comunicação dos resultados;
- comparar alternativas de design presentes no protótipo, com foco no fluxo de seleção de modelos de IA e na apresentação das métricas técnicas exibidas ao usuário.

## Justificativa e Importância

A realização da avaliação é importante para garantir que o GeoSegment AI ofereça uma experiência de uso eficiente, compreensível e adequada aos diferentes perfis de usuários do sistema. Como a plataforma envolve processos técnicos relacionados à inteligência artificial e análise ambiental, é necessário verificar se os usuários conseguem compreender as funcionalidades e interpretar corretamente os resultados apresentados.

Além disso, a avaliação permite identificar problemas de interação e usabilidade antes da implementação final do sistema, reduzindo dificuldades de uso, erros operacionais e possíveis interpretações incorretas das informações geradas pela IA. Também possibilita verificar se o fluxo do sistema é intuitivo e se a interface auxilia o usuário na tomada de decisão durante a escolha dos modelos de segmentação.

Outro ponto relevante é avaliar se as métricas técnicas e os resultados apresentados são comunicados de forma clara, facilitando tanto o uso por especialistas quanto por usuários com menor conhecimento técnico. Dessa forma, a avaliação contribui para melhorar a eficiência do sistema, aumentar a confiabilidade das análises realizadas e tornar a ferramenta mais acessível e adequada ao contexto de aplicação ambiental e acadêmica.

---

# E — Explorar as perguntas da avaliação

Para cada objetivo estabelecido, são definidas perguntas específicas que auxiliam na condução da avaliação e na análise dos resultados obtidos. Essas perguntas levam em consideração os perfis das personas e as atividades realizadas por cada tipo de usuário.

## Perguntas sobre Problemas na Interação e Interface

1 - O usuário consegue realizar o envio de imagens nos formatos (.tif, .png e .jpg) sem necessidade de orientação prévia? Quantos erros ou tentativas incorretas ocorrem durante essa tarefa?<br>
2 - O feedback apresentado pelo sistema durante o processo de upload, como “aguardando”, “processando” e “concluído”, é suficientemente visível e compreensível para o analista ambiental?<br>
3 - O usuário consegue identificar e selecionar o modelo de IA mais adequado (DeepLabV3+ ou V2) a partir das informações exibidas na tela de Seleção de Modelo?<br>
4 - As métricas apresentadas pelo sistema, como precisão e velocidade de processamento, são compreendidas por usuários com menor conhecimento técnico, como o consultor ambiental privado e a gestora de políticas públicas?<br>
5 - O recurso de Comparação Temporal pode ser ativado corretamente sem gerar ambiguidades? O usuário compreende quais informações ou imagens estão sendo comparadas?<br>
6 - O histórico de processamentos disponível na tela Home permite que o usuário localize e retome atividades anteriores de maneira simples e eficiente?<br>
7 - Quais elementos da interface provocam dúvidas, hesitação ou induzem o usuário a cometer erros durante a navegação e execução das tarefas? <br>
8 - O usuário consegue compreender claramente qual deve ser a próxima ação a ser realizada em cada etapa do sistema?<br>

## Perguntas sobre Apropriação de Tecnologia

9 - O consultor ambiental privado consegue realizar a exportação dos dados de cobertura vegetal de forma autônoma para utilização em laudos técnicos?<br>
10 - A gestora de políticas públicas consegue compreender os gráficos e o resumo textual gerados pelo sistema para apoiar apresentações e discussões em reuniões?<br>
11 - O sistema é percebido pelos usuários como uma solução mais eficiente ou vantajosa em relação às ferramentas utilizadas atualmente, como QGIS, ArcGIS e planilhas?<br>
12 - O uso do sistema contribui para tornar as atividades dos usuários mais simples e menos cansativas mentalmente quando comparado ao fluxo de trabalho atual?<br>

## Perguntas sobre Conformidade com Heurísticas

13 - O sistema fornece informações claras e contínuas sobre o andamento do processamento, permitindo que o usuário acompanhe o estado atual das operações realizadas?<br>
14 - Os termos, mensagens e nomenclaturas utilizados na interface são compatíveis com o vocabulário e o contexto dos usuários da área ambiental?<br>
15 - O usuário possui liberdade para cancelar, corrigir ou desfazer ações realizadas incorretamente, como alterar o modelo selecionado antes da conclusão do processamento?<br>
16 - A interface mantém padronização visual e terminológica entre as diferentes telas e funcionalidades do sistema?<br>
17 - O sistema adota mecanismos de prevenção de erros, como validação do formato de arquivos antes do envio das imagens?<br>

## Perguntas sobre Comparação de Alternativas de Design

18 - Qual formato de apresentação das métricas técnicas, texto, tabela ou gráfico facilita mais a compreensão das informações pelos pesquisadores e demais usuários do sistema?<br>
19 - A indicação visual de “Recomendado” no modelo DeepLabV3+ influencia a escolha do usuário durante a seleção do modelo de IA?<br>
20 - Qual organização das informações na tela de Seleção de Modelo torna o processo de escolha mais rápido e intuitivo para os usuários?<br>
21 - Os usuários demonstram maior confiança ao selecionar um modelo quando há explicações adicionais sobre precisão e velocidade?<br>
22 - Qual alternativa de design reduz mais dúvidas e hesitações durante o fluxo de seleção e processamento das imagens?<br>
23 - A forma como os resultados são exibidos permite identificar rapidamente as diferenças entre os modelos disponíveis?<br>

---

# C — Escolher os métodos de avaliação

Os métodos de avaliação foram selecionados com base nas perguntas definidas na seção anterior e nas características atuais do sistema. Como o GeoSegment AI encontra-se em fase de protótipo de alta fidelidade desenvolvido no Figma, torna-se possível realizar tanto avaliações por inspeção quanto avaliações baseadas na observação da interação dos usuários com a interface.

---

## Avaliação Heurística 

**Tipo:** Inspeção, sem participação direta de usuários.<br>

**Objetivo:** Identificar problemas de usabilidade presentes nas telas do protótipo com base nas 10 heurísticas de usabilidade propostas por Jakob Nielsen.<br>

**Escopo:** Avaliação das telas:
- Home
- Upload de Imagem;<br>
- Seleção de Modelo;<br>
- Comparação Temporal;<br>
- Histórico;<br>
- Sobre.<br>

**Avaliadores:** Os 5 integrantes da equipe do projeto atuarão como avaliadores, realizando a inspeção com base nos conhecimentos adquiridos na disciplina de IHC.<br>

**Procedimento:** Cada integrante realizará individualmente a avaliação do protótipo, identificando problemas de usabilidade relacionados às heurísticas de Nielsen. Após as avaliações individuais, os resultados serão reunidos e discutidos em conjunto pela equipe para consolidar os problemas encontrados.<br>

**Dados coletados:**

- lista de problemas encontrados;<br>
- heurística violada;<br>
- nível de severidade do problema;<br>
- descrição do problema.<br>

**Vantagens:** Método de rápida aplicação, baixo custo e que não exige recrutamento de usuários externos.<br>

**Limitações:** A avaliação considera a percepção dos avaliadores e pode não representar completamente o comportamento real dos usuários durante o uso do sistema.<br>

## Teste de Usabilidade com Usuários

**Tipo:** Observação em laboratório com execução de tarefas dirigidas pelos avaliadores.<br>

**Objetivo:** Identificar problemas reais de interação durante o uso do sistema, além de avaliar a eficácia, eficiência e satisfação dos usuários ao realizar as tarefas propostas.<br>
**Escopo:** Avaliação do fluxo completo do sistema, incluindo Upload de Imagem → Seleção de Modelo → Visualização de Resultados, além da funcionalidade de Comparação Temporal.<br>
**Participantes:** Entre 4 e 6 participantes representando os perfis definidos no projeto, incluindo analista ambiental, pesquisadora acadêmica e consultor ambiental privado.<br>
**Ambiente:** Sessões realizadas em laboratório utilizando computador desktop com gravação de tela e áudio, ou de forma remota por plataformas como Zoom e Google Meet, com compartilhamento e gravação da tela.<br>
**Protocolo:** Aplicação da técnica Think-Aloud (pensar em voz alta), em que os participantes verbalizam suas ações, dúvidas e percepções durante a execução das tarefas. As atividades serão apresentadas em sequência previamente definida, sem interferência direta do observador.<br>
**Dados coletados:** Tempo de execução das tarefas, quantidade de erros cometidos, dificuldades observadas, comentários espontâneos dos participantes, momentos de hesitação ou confusão e respostas ao questionário pós-teste SUS (System Usability Scale).<br>

### Questionário Pós-Teste – SUS (System Usability Scale)

Após a realização do teste de usabilidade, os participantes responderão ao questionário SUS (System Usability Scale), proposto por John Brooke, composto por 10 questões em escala Likert de 1 a 5. A aplicação do questionário permitirá obter uma pontuação geral de usabilidade variando de 0 a 100, possibilitando uma avaliação quantitativa da experiência de uso do sistema. O SUS é amplamente utilizado e validado na literatura por fornecer resultados consistentes e comparáveis em avaliações de usabilidade.

---

# I — Identificar e Administrar as Questões Práticas

### Perfil e Número de Participantes

| Persona                     | Perfil Buscado                                                              | Qtd. | Método                 |
|-----------------------------|-----------------------------------------------------------------------------|------|------------------------|
| Analista ambiental          | Analista ambiental ou geógrafo com experiência em monitoramento territorial | 2    | Teste com usuários     |
| Pesquisadora acadêmica      | Pesquisador(a) de visão computacional ou áreas afins                        | 1    | Teste com usuários     |
| Consultor ambiental privado | Consultor ambiental ou técnico de licenciamento ambiental                   | 1–2  | Teste com usuários     |
| Avaliadores de IHC          | Integrantes da equipe com conhecimento em heurísticas de usabilidade        | 5    | Avaliação heurística   |

### Equipamentos necessários

- Computador com acesso à internet e navegador atualizado;
- Protótipo de alta fidelidade no Figma (link compartilhável, modo de apresentação).
- Software de gravação de tela (OBS Studio ou gravação nativa do Zoom);
- Formulários digitais: Termo de Consentimento Livre e Esclarecido (TCLE), questionário pré-teste e questionário SUS pós-teste;
- Planilha de registro de observação para o avaliador anotador;

### Tarefas para o Teste de Usabilidade

| Tarefa | Descrição da Tarefa                                                                                                   | Cenário                         | Funcionalidade                         | Persona(s)                                                        | Tela(s)                     | Perguntas               |
|---------|------------------------------------------------------------------------------------------------------------------------|----------------------------------|----------------------------------------|-------------------------------------------------------------------|------------------------------|--------------------------|
| T1      | Fazer upload de uma imagem aérea para iniciar uma segmentação.                                                        | 1 – Home /<br> 2 – Upload e segmentação | Acesso inicial, upload e processamento | Analista ambiental, consultor                                     | Home / Upload de Imagem      | P1, P2, P7, P8, P13     |
| T2      | Selecionar o modelo considerado mais adequado para a análise.                                                         | 3 – Seleção de modelo           | Seleção de redes neurais               | Pesquisadora acadêmica                                            | Seleção de Modelo            | P3, P4, P16, P17        |
| T3      | Processar a imagem utilizando o modelo selecionado e utilizar a comparação temporal.                                  | 4 – Comparação temporal         | Comparação temporal                    | Analista ambiental, gestora de políticas públicas, consultor      | Comparação Temporal          | P4, P5, P6, P7, P10, P11 |
| T4      | Visualizar e interpretar os resultados da segmentação.                                                                 | 4 – Comparação temporal         | Visualização e interpretação de resultados | Analista ambiental, pesquisadora acadêmica                     | Comparação Temporal          | P4, P5, P10             |
| T5      | Localizar um processamento anterior no histórico e reabrir os resultados.                                              | 5 – Histórico e timeline        | Dashboard inicial / Histórico          | Analista ambiental, consultor                                     | Home / Histórico             | P8, P12                 |
| T6      | Identificar quais modelos o sistema oferece e compreender suas diferenças sem auxílio externo.                         | 3 – Seleção de modelo           | Informações sobre modelos de IA        | Pesquisadora acadêmica                                            | Seleção de Modelo / Sobre    | P3, P4, P16, P17        |


### Recrutamento

- Contato com colegas de curso, professores ou profissionais da área ambiental e de pesquisa conhecidos pelos membros da equipe.
- **Critério de inclusão:** familiaridade mínima com ferramentas web; para perfil técnico, experiência com geoprocessamento ou IA.
- **Critério de exclusão:** membros da equipe de desenvolvimento do GeoSegment.

### Teste-Piloto

Antes da realização das sessões com os participantes, será conduzido um teste-piloto com um integrante da equipe que não tenha participado diretamente do desenvolvimento das telas avaliadas. O objetivo dessa etapa é validar a clareza das instruções fornecidas nas tarefas, verificar o funcionamento dos recursos de gravação utilizados durante a avaliação, estimar a duração média da sessão prevista entre 30 e 45 minutos e analisar se o roteiro e o questionário pós-teste estão adequados para a aplicação definitiva.

---

# D — Decidir sobre as questões éticas

Sempre que usuários são envolvidos em uma avaliação, o avaliador deve tomar os cuidados éticos necessários. Os participantes devem ser respeitados e não podem ser prejudicados direta ou indiretamente, nem durante os experimentos, nem após a divulgação dos resultados.

### Princípios Éticos Adotados:

- **Participação voluntária:** o participante pode interromper a sessão a qualquer momento sem penalidade.- **
- **Anonimato:** os dados coletados serão tratados de forma anônima; nenhum participante será identificado nos relatórios.
- **Consentimento informado:** todos os participantes assinarão o Termo de Consentimento Livre e Esclarecido (TCLE) antes do início da sessão.
- **Transparência:** o objetivo do estudo será explicado claramente — avaliamos o sistema, não o usuário.
- **Proteção de dados:** as gravações serão utilizadas exclusivamente para fins acadêmicos e descartadas após a análise.
- **Ausência de danos:** nenhuma tarefa expõe o participante a conteúdo nocivo; o protótipo é estático e não coleta dados reais.

### Conteúdo do TCLE

O Termo de Consentimento deverá conter: identificação do projeto e da equipe; objetivo da avaliação; descrição das atividades e duração estimada; garantia de anonimato e direito de desistência; uso previsto dos dados coletados; e campo para assinatura/consentimento digital.

---

# E – Avaliar, Interpretar e Apresentar os Dados

### Avaliação Heurística – Interpretação

Cada avaliador registra individualmente os problemas encontrados, associando cada um a uma heurística de Nielsen, à tela afetada e a um grau de severidade:

| Grau | Descrição                                                                 |
|-------|---------------------------------------------------------------------------|
| 0     | Não representa um problema de usabilidade                                 |
| 1     | Problema estético ou cosmético, corrigido apenas se houver disponibilidade |
| 2     | Problema de baixa gravidade, com menor prioridade de correção             |
| 3     | Problema relevante, com alta prioridade de correção                       |
| 4     | Problema crítico, que deve ser corrigido antes da disponibilização do sistema |

Durante a sessão de consolidação, os avaliadores irão discutir coletivamente os problemas identificados para definir, em consenso, o nível de severidade de cada ocorrência. Problemas apontados por dois ou mais avaliadores receberão maior prioridade, por indicarem maior recorrência e relevância durante a avaliação heurística.

### Teste de Usabilidade – Interpretação e Consolidação

#### Análise dos Dados

**Análise qualitativa:** Será realizada a análise das falas registradas durante a aplicação da técnica Think-Aloud, buscando identificar padrões de comportamento, dúvidas frequentes, momentos de hesitação e erros recorrentes apresentados pelos participantes durante a execução das tarefas.
**Análise quantitativa:** Serão analisados indicadores como tempo médio de execução por tarefa, taxa de conclusão das atividades, quantidade média de erros cometidos e pontuação média obtida no questionário SUS (System Usability Scale).
**Análise intersujeito:** Os resultados obtidos com todos os participantes serão consolidados para identificar padrões representativos do grupo, diferenciando dificuldades individuais de problemas recorrentes observados entre múltiplos usuários.

### Validade do Estudo

**Confiabilidade:** A avaliação utilizará um protocolo padronizado, garantindo que todos os participantes executem as mesmas tarefas e recebam as mesmas instruções durante as sessões.
**Validade interna:** Os métodos escolhidos são adequados para avaliar a usabilidade das telas do GeoSegment AI dentro do contexto de uso definido no projeto.
**Validade externa:** Os resultados poderão indicar tendências relevantes sobre a interação com o sistema, porém a generalização deve ser realizada com cautela devido ao número reduzido de participantes e ao recrutamento por conveniência.
**Validade ecológica:** O protótipo desenvolvido no Figma em modo de apresentação aproxima-se da experiência do sistema real, embora não represente completamente fatores como desempenho de rede, processamento real das imagens e execução dos modelos de segmentação.

### Relato dos Resultados

O relatório final da avaliação deverá apresentar:

- os objetivos e o escopo definidos para a avaliação;<br>
- os métodos de avaliação utilizados e suas respectivas justificativas;<br>
- o perfil dos participantes e dos avaliadores envolvidos no estudo;<br>
- o resumo dos dados coletados, incluindo tabelas, resultados do questionário SUS e problemas identificados na avaliação heurística;<br>
- a interpretação e análise dos resultados obtidos, considerando frequência, impacto e severidade dos problemas encontrados;<br>
- uma lista consolidada dos principais problemas de IHC identificados no sistema, organizada por prioridade de correção;<br>
- recomendações de melhorias e reprojeto para cada tela e funcionalidade avaliada.<br>

---

# Considerações finais

A avaliação de IHC do GeoSegment AI tem como objetivo identificar problemas de usabilidade e melhorar a experiência dos usuários antes da implementação final do sistema.
Os métodos escolhidos permitem analisar tanto problemas potenciais da interface quanto dificuldades reais encontradas pelos usuários durante o uso do sistema.
