# Personas

## 1. Ricardo Mendes (Analista Ambiental)
- **Status:** Persona Primária.
- **Identidade:** 42 anos, geógrafo especializado em conservação.
- **Habilidades:** Alta especialidade no domínio ambiental, mas experiência moderada com novas tecnologias de IA.
- **Objetivos:** Realizar o monitoramento ágil da APA de Petrópolis para identificar núcleos urbanos em expansão e fragmentos de vegetação nativa.
- **Tarefas:** Submeter imagens aéreas de alta resolução e exportar estatísticas de proporção por classe para relatórios de fiscalização.
- **Expectativas:** Que a ferramenta seja intuitiva e dispense a instalação de softwares pesados como QGIS.

### Mapa de Empatia
- **O que pensa e sente?** Sente-se sobrecarregado pelo volume de dados; acredita que o mapeamento manual é inviável em larga escala e precisa de agilidade para fiscalização.
- **O que vê?** Imagens aéreas de 30 cm/px com desafios como nuvens e sombras; vê núcleos urbanos avançando sobre a vegetação nativa na APA de Petrópolis.
- **O que ouve?** Colegas discutindo a necessidade de métricas de acurácia mais rigorosas; ouve sobre o potencial da IA para reduzir o trabalho braçal.
- **O que fala e faz?** Elabora relatórios de gestão territorial e utiliza softwares de geoprocessamento tradicionais, mas busca soluções mais leves.
- **Quais são as dores?** A dificuldade técnica de instalar e configurar modelos complexos; a demora no processamento de imagens de alta resolução.
- **Quais são as necessidades?** Uma interface intuitiva onde possa apenas enviar a imagem e receber o mapa e as estatísticas de área.

## 2. Dra. Helena Silveira (Pesquisadora Acadêmica)
- **Status:** Persona Secundária.
- **Identidade:** 35 anos, doutora em Visão Computacional.
- **Habilidades:** Especialista em Aprendizado Profundo e arquiteturas encoder-decoder.
- **Objetivos:** Avaliar a eficácia do modelo DeepLabV3+ em comparação com outras métricas, como a mIoU de referência de 77,75%.
- **Tarefas:** Analisar a qualidade da segmentação em classes desbalanceadas e propor melhorias técnicas no treinamento do modelo.
- **Relacionamentos:** Colabora com órgãos governamentais para validação técnica de ferramentas de IA.

### Mapa de Empatia
- **O que pensa e sente?** Focada na precisão científica; questiona se a arquitetura DeepLabV3+ (V2) é realmente superior à U-Net (V0) em classes desbalanceadas.
- **O que vê?** Gráficos de mIoU e matrizes de confusão; analisa detalhes de bordas entre classes como solo exposto e rocha.
- **O que ouve?** Discussões acadêmicas sobre funções de perda como Focal Loss e Tversky Loss para lidar com amostras reduzidas.
- **O que fala e faz?** Escreve artigos científicos e testa hiperparâmetros; busca reprodutibilidade no fluxo de treinamento.
- **Quais são as dores?** O tamanho limitado do dataset (35 imagens) que pode dificultar a generalização do modelo para outras regiões.
- **Quais são as necessidades?** Acesso a métricas detalhadas (IoU por classe) e transparência nos processos de aumento de dados e validação cruzada.

## 3. Felipe Antunes (Consultor Ambiental de Empresa Privada)
- **Status:** Persona Secundária.
- **Identidade:** 29 anos, trabalha em uma concessionária de rodovias (ex: Ecorodovias).
- **Objetivos:** Obter mapas temáticos rápidos para licenciamento ambiental e análise de impacto em áreas próximas a estradas.
- **Requisitos:** Precisa de escalabilidade para processar várias imagens de alta resolução em curto espaço de tempo.
- **Expectativa:** Que o modelo identifique com precisão as áreas de solo exposto e vegetação esparsa para monitorar obras.

### Mapa de Empatia
- **O que pensa e sente?** Precisa entregar resultados precisos para clientes privados no menor tempo possível para garantir licenciamentos ambientais.
- **O que vê?** A necessidade de identificar fragmentos de vegetação e áreas urbanas em imagens de alta resolução para obras de infraestrutura.
- **O que ouve?** Clientes pressionando por laudos; tendências de mercado sobre o uso de serviços AIaaS (IA como serviço) em nuvem.
- **O que fala e faz?** Analisa áreas de impacto ambiental e exporta mapas temáticos para apresentações comerciais.
- **Quais são as dores?** O alto custo de licenças de softwares como ArcGIS e a necessidade de hardware potente para processamento local.
- **Quais são as necessidades?** Uma ferramenta web estável que não exija instalação e que forneça proporções estatísticas rápidas por classe.

## 4. Cláudia Torres (Gestora de Políticas Públicas / Governo)
- **Status:** Outro Stakeholder (Interessado no resultado, mas não opera a ferramenta diariamente).
- **Identidade:** 50 anos, Secretária de Meio Ambiente.
- **Habilidades:** Baixa experiência técnica com ferramentas de geoprocessamento.
- **Objetivos:** Utilizar os dados agregados (estatísticas de uso do solo) para justificar a criação de novas leis de zoneamento urbano.
- **Dores (Mapa de Empatia):** Sente dificuldade em explicar dados técnicos complexos para a população e outros políticos.
- **Necessidades:** Mapas coloridos e visualmente claros que facilitem a tomada de decisão política.

### Mapa de Empatia
- **O que pensa e sente?** Preocupa-se com o planejamento urbano sustentável; quer dados confiáveis para embasar decisões políticas e leis de zoneamento.
- **O que vê?** Mapas coloridos que facilitam a visualização da cobertura vegetal e das áreas de preservação.
- **O que ouve?** Demandas da sociedade por preservação e pressões para o desenvolvimento urbano na região serrana.
- **O que fala e faz?** Participa de reuniões de conselhos ambientais; utiliza os percentuais de cada classe de solo para justificar investimentos.
- **Quais são as dores?** A dificuldade em interpretar dados técnicos excessivamente complexos ou apresentados de forma pouco visual.
- **Quais são as necessidades?** Visualizações claras (lado a lado) entre a imagem original e o mapa segmentado para facilitar a comunicação com leigos.

## 5. Sr. Benedito (Pequeno Proprietário de Terra)
- **Status:** Persona Extrema (Usuário com perfil de baixa literacia tecnológica e grande impacto emocional pelo produto).
- **Identidade:** 60 anos, produtor rural na região serrana de Petrópolis.
- **Habilidades:** Leigo em tecnologia; utiliza apenas ferramentas básicas de comunicação.
- **Relacionamento com Tecnologia:** Baixa frequência de uso; sente medo de ser prejudicado por análises automáticas incorretas.
- **Expectativas:** Deseja entender se sua área de agricultura está sendo classificada corretamente ou se há risco de multa por invasão de mata nativa.
- **Dores:** Insegurança jurídica em relação à demarcação de sua propriedade.

### Mapa de Empatia
- **O que pensa e sente?** Tem medo de que a tecnologia erre e classifique sua área de agricultura como mata nativa, gerando multas indevidas.
- **O que vê?** Sua terra sendo mapeada por ferramentas digitais que ele não compreende totalmente; vê a fiscalização aumentar na APA de Petrópolis.
- **O que ouve?** Rumores de vizinhos sobre o uso de "computadores que veem tudo do céu" para monitorar as propriedades rurais.
- **O que fala e faz?** Cuida de sua plantação; busca o sindicato rural para entender seus direitos e a demarcação de sua área de agricultura.
- **Quais são as dores?** A exclusão digital e a insegurança jurídica causada por processos de classificação automáticos que ele não pode contestar facilmente.
- **Quais são as necessidades?** Transparência e clareza nos mapas, garantindo que as classes (como agricultura vs. vegetação) sejam distinguidas corretamente.
