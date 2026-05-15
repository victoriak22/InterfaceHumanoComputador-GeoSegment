# HTA – Geração de Insights do Mapa Segmentado

<img width="1438" height="449" alt="image" src="https://github.com/user-attachments/assets/9d90940a-c0d9-4524-ab50-ec15dc333812" />

## Tabela de Problemas e Recomendações

| Objetivos / Operações | Problemas e Recomendações |
|---|---|
| **0. Gerar insights do mapa segmentado (1 → 2 → 3 → 4 → 5)** | **Input:** resultado da segmentação da imagem aérea <br> **Feedback:** visualização de gráficos, estatísticas e relatório exportado <br> **Plano:** acessar dashboard → analisar estatísticas → interpretar resultados → aplicar filtros ou análises adicionais → exportar relatório <br> **Recomendação:** apresentar visualizações claras que facilitem a interpretação dos dados |
| **1. Acessar o Dashboard (1.1 → 1.2)** | **Plano:** abrir aba Insights/Dashboard → carregar resultado da segmentação <br> **Problema:** usuário pode não localizar facilmente a área de visualização dos resultados <br> **Recomendação:** destacar botão ou aba de acesso ao dashboard |
| **1.1 Abrir aba Insights / Dashboard** | **Problema:** navegação entre telas pode ser confusa <br> **Recomendação:** manter menu simples e visível |
| **1.2 Carregar resultado da segmentação** | **Problema:** carregamento lento pode prejudicar a experiência <br> **Recomendação:** otimizar carregamento e indicar progresso |
| **2. Analisar estatísticas (2.1 / 2.2 / 2.3)** | **Plano:** visualizar distribuição por classe, gráfico de pizza e gráfico de barras  <br> **Problema:** excesso de dados pode gerar sobrecarga cognitiva <br> **Recomendação:** destacar informações mais relevantes |
| **2.1 Visualizar distribuição por classe** | **Problema:** usuários podem ter dificuldade em interpretar valores absolutos <br> **Recomendação:** apresentar percentuais de forma clara |
| **2.2 Visualizar gráfico de pizza** | **Problema:** muitos segmentos podem dificultar leitura do gráfico <br> **Recomendação:** agrupar categorias menores |
| **2.3 Visualizar gráfico de barras** | **Problema:** comparação visual pode ser difícil com muitas classes <br> **Recomendação:** ordenar valores ou destacar principais categorias |
| **3. Interpretar resultados (3.1 → 3.2 → 3.3)** | **Plano:** identificar classe dominante → analisar variações → interpretar resumo <br> **Problema:** interpretação pode exigir conhecimento técnico <br> **Recomendação:** incluir resumo interpretativo automático |
| **3.1 Identificar classe dominante** | **Problema:** usuário pode não identificar rapidamente qual classe predomina <br> **Recomendação:** destacar maior valor no gráfico |
| **3.2 Ver variações entre classes** | **Problema:** diferenças pequenas podem passar despercebidas <br> **Recomendação:** usar cores ou indicadores visuais |
| **3.3 Ler resumo interpretativo** | **Problema:** texto pode ser técnico demais <br> **Recomendação:** utilizar linguagem simples e direta |
| **4. Aplicar filtros ou análises adicionais (4.1 / 4.2 / 4.3)** | **Plano:** selecionar período, área de interesse ou atualizar gráficos  <br> **Problema:** muitos filtros podem confundir usuários iniciantes <br> **Recomendação:** fornecer filtros padrão |
| **4.1 Selecionar período** | **Problema:** usuário pode escolher intervalo incorreto <br> **Recomendação:** usar seletor visual de datas |
| **4.2 Selecionar área de interesse** | **Problema:** dificuldade de navegação no mapa <br> **Recomendação:** permitir zoom e seleção interativa |
| **4.3 Atualizar gráficos** | **Problema:** usuário pode não perceber atualização dos dados <br> **Recomendação:** usar animações ou mensagens de atualização |
| **5. Exportar relatório (5.1 → 5.2)** | **Plano:** gerar PDF → salvar relatório <br> **Problema:** processo de exportação pode ser lento <br> **Recomendação:** indicar progresso da exportação |
| **5.1 Gerar PDF** | **Problema:** erro na geração do arquivo pode interromper o processo <br> **Recomendação:** validar dados antes da exportação |
| **5.2 Salvar relatório** | **Problema:** usuário pode não saber onde o arquivo foi salvo <br> **Recomendação:** mostrar local de download ou botão de acesso |
