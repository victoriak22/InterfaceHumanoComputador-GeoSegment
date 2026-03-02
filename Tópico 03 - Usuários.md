# Personas, Mapas de Empatia, Contexto de Uso e Jornada de Usuário

---

## 1. Ricardo Mendes (Analista Ambiental do ICMBio)

### Perfil da Persona
- **Status:** Persona Primária.
- **Perfil:** Geógrafo de 42 anos focado em gestão territorial e fiscalização na APA de Petrópolis.  
- **Objetivos:** Realizar o mapeamento automático do uso do solo para identificar desmatamentos ou expansões urbanas irregulares sem precisar de processamento manual.  
- **Necessidades:** Uma interface web intuitiva que forneça mapas temáticos e proporções estatísticas por classe de forma rápida.

### Mapa de Empatia
- **O que pensa e sente?** Sente que o processamento manual de imagens de alta resolução é inviável em larga escala; busca agilidade para apoiar ações de manejo.  
- **O que vê?** Imagens aéreas de 30 cm/px revelando núcleos urbanos em expansão e fragmentos de vegetação nativa na unidade de conservação.  
- **O que ouve?** Pressões do ICMBio por monitoramento eficiente e decisões embasadas em dados geoespaciais.  
- **O que fala e faz?** Elabora planos de fiscalização e gestão territorial; busca uma ferramenta que dispense instalação de softwares pesados como QGIS.  
- **Quais são as dores?** A dependência de infraestrutura dedicada e o tempo gasto em anotações manuais que retardam a tomada de decisão.  
- **Quais são as necessidades?** Uma interface web intuitiva para visualizar mapas temáticos e consultar proporções de cobertura do solo de forma automática.

### Contexto de Uso: Gestão Territorial
- **Cenário Físico:** Escritório do ICMBio em Petrópolis, com iluminação natural e mapas da unidade de conservação nas paredes. Utiliza um computador desktop padrão conectado à internet.  
- **Narrativa:** Sob pressão para monitorar a expansão de núcleos urbanos na APA de Petrópolis, Ricardo acessa o GeoSegment para processar imagens aéreas de 30 cm/px. O ambiente institucional exige respostas rápidas. A ferramenta em nuvem (AIaaS) permite gerar mapas coloridos e proporções de área por classe sem instalar softwares pesados como ArcGIS ou realizar anotações manuais demoradas.

### Tarefas principais (análise de tarefas)
- Fazer upload de imagem (formato .tiff ou .png) da área de interesse.
- Selecionar e executar a segmentação automática.
- Visualizar mapa original e mapa segmentado lado a lado.
- Acessar estatísticas e proporções por classe.
- Exportar ou utilizar resultados em relatório (com apoio do Dashboard e comparação temporal).

### Jornada de Usuário: Fiscalização
- **Objetivo:** Identificar rapidamente mudanças no uso do solo na APA de Petrópolis para embasar ações de manejo.  
- **Ações:** Abre o navegador → Carrega uma imagem de alta resolução (30 cm/px) → Solicita a segmentação automática → Analisa a visualização lado a lado (Original vs. Segmentado).  
- **Pensamentos:**  
  - "Preciso desses dados estatísticos agora para o relatório de fiscalização."  
  - "Ainda bem que não preciso configurar o QGIS para processar esse volume de dados."  
- **Emoções:** Urgência → Expectativa durante o processamento → Alívio e segurança profissional ao obter o mapa temático.

---

## 2. Dra. Helena Silveira (Pesquisadora Acadêmica)

### Perfil da Persona
- **Status:** Persona Primária.
- **Perfil:** Doutora em Visão Computacional, 35 anos, interessada na validade científica dos modelos de IA.  
- **Objetivos:** Comparar o desempenho das arquiteturas (V0, V1 e V2) e validar métricas como mIoU e IoU por classe.  
- **Necessidades:** Acesso a resultados de segmentação em nível de pixel e compreensão de como o modelo lida com classes desbalanceadas e refinamento de bordas.

### Mapa de Empatia
- **O que pensa e sente?** Preocupa-se com o rigor científico; questiona se o DeepLabV3+ mantém precisão comparável ao benchmark V0.  
- **O que vê?** Gráficos de desempenho, arquiteturas encoder-decoder e a distribuição de classes nos folds de validação cruzada.  
- **O que ouve?** Discussões sobre AIaaS e métricas avançadas como Boundary IoU.  
- **O que fala e faz?** Compara sistematicamente modelos (V0, V1 e V2) e analisa o impacto das funções de perda (Focal Loss + Dice Loss).  
- **Quais são as dores?** Desbalanceamento severo de classes minoritárias como Água e Rocha em dataset reduzido.  
- **Quais são as necessidades?** Métricas detalhadas por classe e experimentos reproduzíveis.

### Contexto de Uso: Validação de Modelos
- **Cenário Físico:** Laboratório de computação silencioso com estação de trabalho e dois monitores de alta fidelidade cromática.  
- **Narrativa:** Helena analisa tecnicamente as versões V0, V1 e V2 do sistema. Precisa justificar o uso do modelo V2 (DeepLabV3+) mesmo com mIoU de 73,81% inferior ao benchmark V0 (77,75%). Ela examina erros em classes desbalanceadas e avalia se a função de perda composta melhorou o refinamento de bordas.

### Tarefas principais (análise de tarefas)
- Fazer upload de imagens ou patches para teste (ex.: classes Água e Rocha).
- Selecionar a rede neural (V0, V1 ou V2) e ver informações técnicas (métricas, arquitetura).
- Analisar resultado de segmentação em nível de pixel.
- Comparar desempenho entre modelos (mIoU, IoU por classe, refinamento de bordas).
- Documentar ou exportar resultados para publicação.

### Jornada de Usuário: Validação Técnica
- **Objetivo:** Validar cientificamente o modelo V2 para publicação de resultados.  
- **Ações:** Acessa a interface → Envia patches com Água e Rocha → Analisa segmentação pixel a pixel → Compara resultados com métricas de referência.  
- **Pensamentos:**  
  - "Será que a arquitetura mais leve compensa a pequena perda de mIoU?"  
  - "O refinamento de bordas parece melhor."  
- **Emoções:** Ceticismo científico → Concentração profunda → Confiança no modelo.

---

## 3. Felipe Antunes (Consultor Ambiental Privado)

### Perfil da Persona
- **Status:** Persona Secundária.
- **Perfil:** Consultor ambiental de 29 anos que trabalha para empresas de infraestrutura.  
- **Objetivos:** Obter laudos rápidos de cobertura vegetal para licenciamento ambiental.  
- **Necessidades:** Escalabilidade e acesso ao modelo como serviço (AIaaS).

### Mapa de Empatia
- **O que pensa e sente?** Valoriza produtividade e rapidez para atender clientes.  
- **O que vê?** Plataformas web capazes de simplificar fluxos complexos de inferência.  
- **O que ouve?** Que softwares tradicionais são caros e exigem treinamento longo.  
- **O que fala e faz?** Analisa áreas comerciais e exporta mapas para relatórios técnicos.  
- **Quais são as dores?** Alto custo de hardware e licenças como ArcGIS.  
- **Quais são as necessidades?** Processamento sob demanda e integração fácil com laudos.

### Contexto de Uso: Consultoria Privada
- **Cenário Físico:** Escritório open office movimentado. Usa notebook corporativo alternando entre Wi-Fi e 4G.  
- **Narrativa:** Felipe precisa entregar rapidamente um relatório de cobertura vegetal para uma concessionária. Usa o GeoSegment para processar recortes de imagens e obter percentuais de classes para laudos ambientais.

### Tarefas principais (análise de tarefas)
- Acessar o sistema e ver histórico/timeline de processamentos.
- Fazer upload de imagens das áreas de interesse.
- Obter segmentação e estatísticas por classe.
- Copiar ou exportar dados para planilhas e laudos.

### Jornada de Usuário: Produtividade
- **Objetivo:** Gerar rapidamente dados de cobertura vegetal para relatórios.  
- **Ações:** Acessa o GeoSegment → Faz upload das áreas → Copia estatísticas para planilha.  
- **Pensamentos:**  
  - "Isso economiza horas de trabalho manual."  
- **Emoções:** Pressão por prazos → Foco → Entusiasmo com a agilidade.

---

## 4. Cláudia Torres (Gestora de Políticas Públicas)

### Perfil da Persona
- **Status:** Stakeholder.
- **Perfil:** Secretária de Meio Ambiente, 50 anos, focada em planejamento urbano estratégico.  
- **Objetivos:** Utilizar dados e mapas para embasar decisões políticas e leis de zoneamento.  
- **Necessidades:** Visualizações claras e estatísticas compreensíveis.

### Mapa de Empatia
- **O que pensa e sente?** Preocupada com o zoneamento sustentável e preservação ambiental.  
- **O que vê?** Mapas coloridos que facilitam a leitura territorial.  
- **O que ouve?** Demandas por transparência na gestão ambiental.  
- **O que fala e faz?** Apresenta diagnósticos territoriais e propõe políticas públicas.  
- **Quais são as dores?** Dificuldade em interpretar dados técnicos complexos.  
- **Quais são as necessidades?** Visualizações comparativas e estatísticas claras.

### Contexto de Uso: Planejamento Estratégico
- **Cenário Físico:** Sala de reuniões da Secretaria de Meio Ambiente com projetor exibindo resultados.  
- **Narrativa:** Cláudia lidera discussões sobre zoneamento urbano utilizando mapas gerados pelo sistema para demonstrar áreas críticas e justificar decisões políticas.

### Jornada de Usuário: Comunicação Estratégica
- **Objetivo:** Apresentar dados claros para decisões de políticas públicas.  
- **Ações:** Observa a operação do sistema → Analisa mapas projetados → Apresenta estatísticas ao conselho.  
- **Pensamentos:**  
  - "As cores facilitam o entendimento do avanço urbano."  
- **Emoções:** Preocupação → Determinação → Autoridade técnica.

---

## 5. Sr. Benedito (Pequeno Proprietário Rural)

### Perfil da Persona
- **Status:** Persona Extrema.
- **Perfil:** Produtor rural de 60 anos da região serrana de Petrópolis.  
- **Objetivos:** Garantir que sua área agrícola seja classificada corretamente.  
- **Necessidades:** Transparência e precisão no mapeamento.

### Mapa de Empatia
- **O que pensa e sente?** Receio de ser prejudicado por erros da tecnologia.  
- **O que vê?** Sua propriedade identificada por imagens aéreas.  
- **O que ouve?** Comentários sobre fiscalização ambiental automatizada.  
- **O que fala e faz?** Trabalha na terra e busca entender o funcionamento do sistema.  
- **Quais são as dores?** Possível confusão entre Agricultura e Vegetação Esparsa.  
- **Quais são as necessidades?** Alta precisão e clareza no processo.

### Contexto de Uso: Verificação de Conformidade
- **Cenário Físico:** Varanda de casa rural com internet instável via rádio.  
- **Narrativa:** O neto ajuda o Sr. Benedito a visualizar o mapa da propriedade. Ele observa se a área agrícola foi corretamente identificada.

### Jornada de Usuário: Segurança Jurídica
- **Objetivo:** Confirmar que sua área de cultivo está correta no sistema.  
- **Ações:** Solicita ajuda ao neto → Visualiza o mapa segmentado → Confere os limites da propriedade.  
- **Pensamentos:**  
  - "Espero que a tecnologia não me prejudique."  
- **Emoções:** Desconfiança → Ansiedade → Alívio ao confirmar a classificação correta.

---

## Rastreabilidade: Persona → Telas e fluxos principais (Tópico 11)

| Persona | Telas / fluxos principais no GeoSegment |
|---------|----------------------------------------|
| Ricardo Mendes | Home inicial → Upload de imagem → Seleção de rede → Dashboard (insights, estatísticas, comparação temporal, relatório) |
| Dra. Helena Silveira | Upload de imagem → Seleção de rede (com informações técnicas e métricas) → Dashboard (análise pixel a pixel, comparação de modelos) |
| Felipe Antunes | Home inicial → Upload → Seleção de rede → Dashboard (estatísticas, exportação para laudos); uso frequente do histórico/timeline |
| Cláudia Torres | Dashboard (visualizações, gráficos, relatório em linguagem acessível para apresentação em reuniões) |
| Sr. Benedito | Visualização do mapa segmentado da propriedade (com apoio); confirmação de classificação da área agrícola |
