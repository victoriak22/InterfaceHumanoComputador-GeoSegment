# HTA – Seleção de Modelo de Rede Neural

<img width="1482" height="367" alt="image" src="https://github.com/user-attachments/assets/3c54a43a-989a-4d58-83c3-6fe14b80e9f9" />

# HTA – Seleção de Modelo de Rede Neural
## Tabela de Problemas e Recomendações

| Objetivos / Operações | Problemas e Recomendações |
|---|---|
| **0. Selecionar modelo de rede neural (1 > 2 > 3 > 4)** | **Input:** imagem previamente carregada no sistema <br> **Feedback:** confirmação do modelo selecionado e execução da segmentação <br> **Plano:** acessar tela de seleção → analisar modelos disponíveis → comparar desempenho → selecionar modelo <br> **Recomendação:** apresentar informações técnicas de forma clara e acessível para diferentes níveis de usuários |
| **1. Acessar a tela de seleção de modelo (1.1 > 1.2)** | **Plano:** finalizar upload da imagem → acessar página de seleção de rede <br> **Problema:** usuário pode não saber onde acessar a seleção de modelos <br> **Recomendação:** mostrar claramente a próxima etapa após o upload |
| **1.1 Finalizar upload da imagem** | **Problema:** usuário pode tentar acessar seleção de modelo antes do upload terminar <br> **Recomendação:** bloquear acesso até conclusão do upload |
| **1.2 Ir para página Seleção de Rede** | **Problema:** navegação entre etapas pode ser confusa <br> **Recomendação:** indicar fluxo de navegação guiado |
| **2. Analisar modelos disponíveis (2.1 / 2.2 / 2.3)** | **Plano:** visualizar arquiteturas → visualizar descrição → visualizar métricas de referência (em qualquer ordem) <br> **Problema:** usuários não especialistas podem ter dificuldade em compreender modelos de IA <br> **Recomendação:** fornecer explicações simplificadas e exemplos de uso |
| **2.1 Visualizar lista de arquiteturas (V0, V1, V2)** | **Problema:** excesso de opções pode gerar dúvida na escolha <br> **Recomendação:** destacar modelo recomendado |
| **2.2 Visualizar descrição da arquitetura** | **Problema:** descrição pode conter termos técnicos difíceis <br> **Recomendação:** incluir resumo simplificado ou tooltip explicativo |
| **2.3 Visualizar métricas de referência** | **Problema:** métricas podem ser difíceis de interpretar <br> **Recomendação:** apresentar gráficos comparativos de desempenho |
| **3. Comparar desempenho (3.1 / 3.2 / 3.3)** | **Plano:** analisar métricas de desempenho em qualquer ordem <br> **Problema:** comparação de várias métricas pode gerar sobrecarga cognitiva <br> **Recomendação:** destacar diferenças principais entre os modelos |
| **3.1 Visualizar mIoU geral** | **Problema:** usuários podem não compreender o significado da métrica mIoU <br> **Recomendação:** incluir explicação da métrica |
| **3.2 Visualizar IoU por classe** | **Problema:** grande quantidade de classes pode dificultar análise <br> **Recomendação:** destacar classes mais relevantes |
| **3.3 Avaliar refinamento de bordas** | **Problema:** avaliação visual pode ser difícil sem comparação direta <br> **Recomendação:** mostrar exemplos comparativos entre modelos |
| **4. Selecionar modelo (4.1 → 4.2)** | **Plano:** escolher rede → confirmar seleção <br> **Problema:** usuário pode escolher modelo inadequado <br> **Recomendação:** sugerir configuração padrão baseada no tipo de análise |
| **4.1 Escolher rede desejada** | **Problema:** decisão pode ser difícil sem experiência técnica <br> **Recomendação:** indicar casos de uso para cada modelo |
| **4.2 Confirmar seleção** | **Problema:** usuário pode confirmar seleção por engano <br> **Recomendação:** exibir resumo da escolha antes da confirmação |
