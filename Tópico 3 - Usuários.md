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

### Contexto de Uso
- **Cenário Físico:** Ricardo trabalha em uma sala arejada na sede do ICMBio, sentado em uma mesa ergonômica com dois monitores grandes para facilitar a visualização de detalhes espaciais.
- **Narrativa:** É manhã de segunda-feira e Ricardo precisa validar uma denúncia de desmatamento na APA de Petrópolis. Ele abre o navegador e acessa o GeoSegment. O ambiente social é de foco; ele não quer lidar com a complexidade técnica de softwares locais como o QGIS. Ricardo faz o upload de uma imagem de 30 cm/px e, enquanto toma seu café, observa a barra de progresso. Ao ver o mapa segmentado lado a lado com a imagem original, ele identifica rapidamente que uma área de Vegetação Densa foi convertida em Solo Exposto, confirmando a infração através das estatísticas geradas automaticamente pela plataforma.

### Jornada de Usuário
- **Objetivo:** Identificar rapidamente um possível desmatamento na APA de Petrópolis para gerar um auto de infração.
- **Ações:** Acessa o navegador -> Entra no site do GeoSegment -> Faz o upload da imagem de alta resolução (30 cm/px) -> Clica em "Processar Segmentação" -> Analisa o mapa temático comparando-o com a imagem original.
- **Pensamentos:** "Preciso que esse modelo seja preciso nas bordas da vegetação densa." "Ainda bem que não precisei configurar o QGIS para isso".
- **Emoções:** Ansiedade pelo prazo de fiscalização -> Curiosidade durante o processamento -> Alívio e confiança ao ver a classe "Solo Exposto" claramente identificada onde antes havia floresta.

## 2. Dra. Helena Silveira (Pesquisadora Acadêmica)
- **Status:** Persona Secundária.
- **Identidade:** 35 anos, doutora em Visão Computacional.
- **Habilidades:** Especialista em Aprendizado Profundo e arquiteturas encoder-decoder.
- **Objetivos:** Avaliar a eficácia do modelo DeepLabV3+ em comparação com outras métricas, como a mIoU de referência de 77,75%.
- **Tarefas:** Analisar a qualidade da segmentação em classes desbalanceadas e propor melhorias técnicas no treinamento do modelo.
- **Relacionamentos:** Colabora com órgãos governamentais para validação técnica de ferramentas de IA.

### Mapa de Empatia
- **O que pensa e sente?** Focada na precisão científica; questiona se a arquitetura utilizada respodende com resuktados plausíveis.
- **O que vê?** Gráficos de acuracidade e metricas que comporvam o resultado obtido; analisa detalhes de bordas entre classes como solo exposto e rocha.
- **O que ouve?** Discussões acadêmicas sobre funções de perda com amostras reduzidas.
- **O que fala e faz?** Escreve artigos científicos e testa hiperparâmetros; busca reprodutibilidade no fluxo de treinamento.
- **Quais são as dores?** O tamanho limitado do dataset que pode dificultar a generalização do modelo para outras regiões.
- **Quais são as necessidades?** Acesso a métricas detalhadas (acuracidade por classe) e transparência nos processos de aumento de dados e validação cruzada.

### Contexto de Uso
- **Cenário Físico:** Um laboratório acadêmico silencioso, com iluminação controlada para evitar reflexos nas telas. Ela utiliza uma estação de trabalho de alto desempenho.
- **Narrativa:** Helena está revisando os resultados do modelo DeepLabV3+ para um artigo científico. Ela analisa o comportamento do modelo em regiões de bordas e transições abruptas. No contexto social, ela interage com alunos de pós-graduação, discutindo por que o mIoU de 73,81% da DeepLabV3+ é preferível para a interface web devido à menor latência de inferência, apesar de ser ligeiramente inferior ao benchmark . Ela utiliza a interface para realizar testes de estresse com patches de imagens que possuem classes desbalanceadas, como Água e Rocha.

### Jornada de Usuário
- **Objetivo:** Validar se a arquitetura DeepLabV3+ com backbone ResNet-101 mantém a consistência em classes minoritárias como "Água".
- **Ações:** Abre a plataforma -> Sobe amostras específicas com presença de corpos d'água e rocha -> Observa a segmentação em nível de pixel -> Compara os percentuais gerados com seus dados de referência.
- **Pensamentos:** "Será que o Combo Loss da DeepLabV3+ realmente penalizou os erros nas classes desbalanceadas?" "A latência de inferência parece menor que a da U-Net".
- **Emoções:** Ceticismo científico -> Concentração profunda -> Satisfação ao notar que o refinamento de bordas está superior às versões anteriores.

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

### Contexto de Uso
- **Cenário Físico:** Escritório moderno de uma grande empresa (ex: Ecorodovias), em um ambiente agitado com telefones tocando e prazos curtos.
- **Narrativa:** Felipe precisa finalizar um laudo de impacto ambiental para uma nova obra viária até o fim do dia. Ele utiliza um notebook corporativo conectado ao Wi-Fi da empresa. O contexto é de alta pressão por produtividade. Em vez de esperar dias pelo processamento de uma equipe de geoprocessamento externa, ele mesmo sobe os recortes da área de interesse no GeoSegment. A facilidade de obter as proporções por classe (como área urbana vs. vegetação esparsa) permite que ele preencha as tabelas do relatório técnico de forma instantânea, garantindo a entrega no prazo.

### Jornada de Usuário
- **Objetivo:** Obter dados estatísticos de ocupação urbana para um laudo de licenciamento de rodovias.
- **Ações:** Abre o notebook no meio de uma reunião -> Acessa a API do GeoSegment -> Faz o upload do recorte da área da obra -> Copia os valores percentuais das classes "Urbano" e "Vegetação Esparsa" diretamente para sua planilha.
- **Pensamentos:** "Se eu tivesse que esperar o setor de geoprocessamento processar isso, levaria dias." "O visual desse mapa colorido vai impressionar o cliente".
- **Emoções:** Estresse pela urgência do laudo -> Pressa -> Entusiasmo com a agilidade da entrega dos resultados via web.

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

### Contexto de Uso
- **Cenário Físico:** Uma sala de reuniões da prefeitura, com um projetor exibindo dados para uma comissão de planejamento urbano.
- **Narrativa:** Cláudia apresenta o plano de zoneamento para os próximos cinco anos. O ambiente é formal e exige clareza visual para convencer outros secretários. Ela não opera a ferramenta, mas utiliza os resultados exportados: o mapa temático colorido onde o Vermelho (Urbano) e o Verde Escuro (Vegetação Densa) criam um contraste óbvio sobre onde o crescimento deve ser limitado. Ela aponta para os gráficos de pizza gerados pela interface, usando o dado de "13,2 km² de área monitorada" para justificar novos investimentos em preservação na região serrana.

### Jornada de Usuário
- **Objetivo:** Convencer a comissão de planejamento sobre a necessidade de novas zonas de preservação.
- **Ações:** Solicita ao técnico que abra o GeoSegment no projetor da sala -> Aponta para o contraste entre o vermelho (Urbano) e o verde (Vegetação Densa) -> Destaca o gráfico de áreas totais monitoradas (13,2 km²).
- **Pensamentos:** "Este mapa torna o problema do crescimento urbano óbvio para qualquer leigo." "Os dados automáticos dão mais autoridade à minha proposta".
- **Emoções:** Preocupação com o zoneamento -> Determinação -> Senso de dever cumprido ao ver os membros da comissão entenderem os dados visuais.

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

### Contexto de Uso
- **Cenário Físico:** Uma área rural na APA de Petrópolis. Ele está sentado na varanda de sua casa, tentando usar um tablet com conexão 4G instável.
- **Narrativa:** Preocupado com notícias sobre multas ambientais, o Sr. Benedito pede ao neto para mostrar "como o governo está vendo a terra dele". O contexto social é de desconfiança e ansiedade em relação à tecnologia automática. Ele observa o mapa gerado e busca identificar sua plantação de Agricultura (Amarelo). Para ele, o sucesso do uso é o sentimento de alívio ao perceber que o sistema não confundiu sua área de cultivo com mata nativa preservada, garantindo que ele está em conformidade com as regras da unidade de conservação.

### Jornada de Usuário
- **Objetivo:** Conferir se sua área de plantio não está sendo confundida com floresta nativa pelo sistema do governo.
- **Ações:** Pede ao neto para acessar o site -> Observa a tela enquanto a imagem de sua fazenda é processada -> Busca a cor amarela (Agricultura) no mapa segmentado.
- **Pensamentos:** "Espero que esse computador saiba a diferença entre o meu pomar e a mata fechada." "Não quero receber uma multa por algo que eu não fiz".
- **Emoções:** Desconfiança e medo da tecnologia -> Tensão -> Tranquilidade ao ver que o "Amarelo" respeitou os limites da sua lavoura.
