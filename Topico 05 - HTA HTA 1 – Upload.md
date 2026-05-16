# HTA – Upload e Segmentação de Imagens

<img width="1032" height="334" alt="image" src="https://github.com/user-attachments/assets/da3bebf8-db33-42e9-9e0b-fd4762f572b4" />


## Tabela de Problemas e Recomendações

| Objetivos / Operações | Problemas e Recomendações |
|---|---|
| **0. Upload e Segmentação de Imagens (1 → 2 → 3 → 4 → 5)** | **Input:** imagem aérea de alta resolução (.tiff ou .png) <br> **Feedback:** exibição do mapa segmentado e estatísticas por classe ou histórico.<br> **Plano:** acessar sistema → realizar upload → validar arquivo → executar segmentação → visualizar resultados <br> **Recomendação:** permitir acesso via navegador sem necessidade de softwares especializados |
| **1. Acessar o sistema GeoSegment (1.1 → 1.2 → 1.3)** | Plano: abrir navegador e acessar sistema <br> Problema: usuários podem ter dificuldades para acessar a interface ou conexão instável <br> Recomendação: interface web simples e compatível com navegadores comuns |
| **1.1 Abrir navegador web** | Problema: navegador incompatível pode afetar funcionamento do sistema <br> Recomendação: indicar navegadores recomendados |
| **1.2 Digitar endereço do sistema** | Problema: erro ao digitar a URL pode impedir acesso <br> Recomendação: disponibilizar acesso via link direto ou favoritos |
| **1.3 Acessar tela inicial** | Problema: usuário pode não identificar rapidamente onde iniciar a tarefa <br> Recomendação: destacar botão principal de upload ou iniciar análise |
| **2. Iniciar processo de upload (2.1 → 2.2 → 2.3)** | Plano: selecionar imagem e iniciar envio <br> Problema: arquivos grandes podem causar lentidão no envio <br> Recomendação: exibir barra de progresso durante o upload |
| **2.1 Clicar na opção Upload de imagem** | Problema: botão pode não ser facilmente identificado <br> Recomendação: destacar botão principal de upload na interface |
| **2.2 Selecionar arquivo no computador** | Problema: usuário pode escolher arquivo incorreto <br> Recomendação: mostrar pré-visualização do arquivo selecionado |
| **2.3 Verificar formato aceito (.tiff, .png)** | Problema: usuário pode tentar enviar formatos inválidos <br> Recomendação: restringir seleção apenas aos formatos compatíveis |
| **3. Validar arquivo enviado (3.1 → 3.2 → 3.3)** | Plano: sistema valida o arquivo e confirma envio <br> Problema: usuário pode não saber se o upload foi concluído <br> Recomendação: exibir status claro de validação |
| **3.1 Sistema verifica tamanho e formato** | Problema: arquivos muito grandes podem gerar erro <br> Recomendação: informar limites de tamanho antes do envio |
| **3.2 Sistema mostra barra de progresso** | Problema: ausência de indicador pode gerar incerteza no usuário <br> Recomendação: mostrar progresso visual do upload |
| **3.3 Sistema confirma upload** | Problema: usuário pode não perceber que o envio foi concluído <br> Recomendação: exibir mensagem de confirmação clara |
| **4. Executar segmentação** | Plano: iniciar processamento da imagem <br> Problema: tempo de processamento pode ser elevado <br> Recomendação: exibir status do processamento e tempo estimado |
| **5. Visualizar resultado (5.1 → 5.2)** | Plano: apresentar resultados da análise <br> Problema: excesso de informação pode dificultar interpretação <br> Recomendação: apresentar gráficos e visualizações claras |
| **5.1 Analisar estatísticas (5.1.1 / 5.1.2)** | Problema: dados numéricos podem ser difíceis de interpretar <br> Recomendação: usar gráficos e porcentagens simplificadas |
| **5.1.1 Analisar estatísticas por histórico** | Problema: dificuldade em identificar mudanças ao longo do tempo <br> Recomendação: permitir comparação temporal |
| **5.1.2 Analisar estatísticas por classe** | Problema: interpretação da distribuição das classes <br> Recomendação: destacar proporções por classe de uso do solo |
| **5.2 Visualizar mapas lado a lado** | Problema: dificuldade em comparar visualmente os mapas <br> Recomendação: permitir zoom, sincronização e alternância de camadas |
