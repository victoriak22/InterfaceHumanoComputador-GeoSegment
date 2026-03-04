# Análise Hierárquica de Tarefas (HTA) – GeoSegment

Este documento descreve a Análise Hierárquica de Tarefas (HTA) do projeto **GeoSegment**, relacionando objetivos/operações com problemas e recomendações de usabilidade.

## Diagrama HTA

A estrutura hierárquica das tarefas do sistema é representada no diagrama abaixo:

![Diagrama HTA - GeoSegment](https://github.com/user-attachments/assets/3a861d3e-10d5-416b-940b-aa7f5f785fed)

---

| Objetivos / Operações | Problemas e Recomendações |
|----------------------|---------------------------|
| **0. Analisar uso do solo a partir de imagem aérea (1>2>3>4)** | **Input:** imagem aérea de alta resolução (ex.: 30 cm/px)<br>**Feedback:** exibição do mapa segmentado e estatísticas por classe<br>**Plano:** carregar imagem → configurar segmentação → executar processamento → analisar resultados<br>**Recomendação:** permitir acesso via navegador sem necessidade de softwares especializados |
| **1. Carregar imagem da área de interesse (1>1.1>1.2)** | **Plano:** selecionar arquivo e confirmar upload<br>**Problema:** arquivos grandes podem gerar lentidão ou falhas<br>**Recomendação:** exibir barra de progresso e validação automática de formato e resolução |
| **1.1 Selecionar arquivo (.tiff ou .png)** | **Problema:** usuário pode tentar enviar formatos inválidos<br>**Recomendação:** restringir seleção apenas a formatos compatíveis |
| **1.2 Confirmar upload da imagem** | **Feedback:** pré-visualização da imagem carregada<br>**Recomendação:** permitir cancelamento ou substituição da imagem |
| **2. Configurar segmentação automática (depende de 1)** | **Plano:** selecionar modelo de IA e parâmetros de execução<br>**Problema:** usuários não especialistas podem não compreender termos técnicos<br>**Recomendação:** fornecer descrições simplificadas e tooltips |
| **2.1 Selecionar modelo de segmentação (V0, V1 ou V2)** | **Problema:** dificuldade em decidir qual modelo utilizar<br>**Recomendação:** apresentar métricas resumidas e indicação de uso recomendado |
| **2.2 Definir parâmetros de execução** | **Problema:** excesso de opções pode confundir usuários leigos<br>**Recomendação:** oferecer configurações padrão e modo avançado opcional |
| **3. Executar segmentação automática (depende de 1 e 2)** | **Ação:** iniciar processamento de inferência<br>**Problema:** tempo de espera elevado pode gerar ansiedade<br>**Recomendação:** exibir status do processamento e tempo estimado |
| **4. Visualizar resultados da segmentação (depende de 1, 2 e 3)** | **Plano:** visualizar mapas e estatísticas simultaneamente<br>**Problema:** sobrecarga de informação visual<br>**Recomendação:** permitir personalização do dashboard |
| **4.1 Analisar estatísticas** | **Problema:** dados numéricos podem ser difíceis de interpretar<br>**Recomendação:** uso de gráficos e percentuais simplificados |
| **4.1.1 Analisar estatísticas por histórico** | **Problema:** dificuldade em identificar mudanças ao longo do tempo<br>**Recomendação:** permitir comparação temporal quando disponível |
| **4.1.2 Analisar estatísticas por classe** | **Problema:** interpretação da distribuição das classes<br>**Recomendação:** destacar proporções por classe de uso do solo |
| **4.2 Visualizar mapas lado a lado** | **Feedback:** mapas coloridos facilitam a interpretação espacial<br>**Recomendação:** permitir zoom, sincronização e alternância de camadas |

