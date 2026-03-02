# Tópico 4 – Cenário de Análise de Problemas

Cada uma das **cinco grandes funcionalidades** do sistema (Tópico 01) possui um cenário de análise de problemas, vinculado ao integrante responsável e à(s) persona(s) correspondente(s). Em cada cenário utilizam-se os **elementos da técnica de cenários**: **objetivo** (o que se quer alcançar), **ambiente** (onde e quando ocorre), **atores** (quem participa), **planejamento** (ordem e condições), **ação** (o que o usuário faz), **evento** (o que o sistema faz ou responde) e **avaliação** (como se verifica o sucesso e o resultado).

---

## Cenário 1 – Upload e segmentação de imagens (Vinicius Saidi Soares)

**Funcionalidade (Tópico 01):** Segmentação de imagens – upload e processamento.  
**Título:** Necessidade de carregar imagens de forma rápida e confiável para segmentação semântica.  
**Atores:** Ricardo Mendes (analista ambiental do ICMBio), Sistema GeoSegment.

**Cenário inicial:** Ricardo precisa enviar uma imagem aérea (ex.: .tiff ou .png) da APA de Petrópolis para obter o mapa segmentado. Hoje depende de ferramentas locais ou processos manuais. Objetivo: reduzir tempo e garantir que o formato e o tamanho do arquivo sejam aceitos, com feedback claro de progresso.

**Cenário refinado:** Ricardo acessa a Home do GeoSegment e segue para a tela de Upload. Seleciona o arquivo; o sistema informa o status (upload em andamento, validação). Após o upload, pode escolher a rede (Cenário 2) e disparar a segmentação. O sistema exibe indicador de processamento e, ao concluir, leva à visualização (original vs. segmentado). Avaliação: upload concluído sem erro, resultado visível em tempo hábil.

**Problema evidenciado:** Dependência de softwares locais; falta de feedback durante o processamento. **Valor da interface:** Acesso web, upload direto, visibilidade do status e resultado integrado (telas: Home, Upload de imagem; ver Tópico 11).

---

## Cenário 2 – Seleção de rede neural e validação técnica (Gustavo Dias Vicentin)

**Funcionalidade (Tópico 01):** Seleção de redes neurais e informações técnicas.  
**Título:** Pesquisadora precisa escolher o modelo e acessar métricas para validação científica.  
**Atores:** Dra. Helena Silveira (pesquisadora), Sistema GeoSegment.

**Cenário inicial:** Helena precisa comparar as arquiteturas (V0, V1, V2) e justificar o uso do modelo em publicação. Necessita saber qual rede está em uso, ver parâmetros e métricas (ex.: mIoU, IoU por classe) sem configurar ambiente local.

**Cenário refinado:** Após o upload (Cenário 1), Helena acessa a tela de Seleção de rede. Escolhe o modelo (ex.: DeepLabV3+ / V2), visualiza informações técnicas (rede em uso, métricas de referência). Dispara a segmentação e analisa o resultado no Dashboard, com foco em classes desbalanceadas e refinamento de bordas. Avaliação: decisão embasada em dados técnicos visíveis na própria interface.

**Problema evidenciado:** Falta de transparência sobre qual modelo está sendo usado e quais métricas sustentam a escolha. **Valor da interface:** Controle do modelo e acesso a informações técnicas na mesma ferramenta (telas: Upload, Seleção de rede, Dashboard; ver Tópico 11).

---

## Cenário 3 – Geração de Insights e Painéis para Apoio à Decisão Territorial (Deise Adriana Silva Araújo)

**Funcionalidade (Tópico 01):** Geração de insights e painéis (dashboards).  
**Título do cenário:** Dificuldade na interpretação de resultados técnicos de segmentação para tomada de decisão estratégica.

**Atores:** Ricardo Mendes (analista ambiental do ICMBio), Cláudia Torres (gestora de políticas públicas), Sistema GeoSegment (interface web com dashboards).

**Elementos da técnica neste cenário:** Objetivo – obter estatísticas e insights a partir do mapa segmentado para relatório e apresentação; Ambiente – escritório ICMBio e reunião na Secretaria; Atores – Ricardo, Cláudia, sistema; Ação – acessar aba Insights/Dashboard, ativar comparação temporal, exportar PDF; Evento – gráficos atualizam, resumo interpretativo é gerado; Avaliação – relatório entregue no prazo, decisão tomada na reunião.

---

### 1. Cenário inicial (antes do refinamento)

Ricardo Mendes está no escritório do ICMBio em Petrópolis, com prazo curto para entregar um relatório sobre avanço urbano na APA. Ele já realizou a segmentação automática de uma imagem aérea de alta resolução no GeoSegment e o sistema gerou o mapa segmentado corretamente. Mesmo assim, Ricardo precisa responder perguntas estratégicas: qual porcentagem da área corresponde a vegetação nativa, se houve aumento de área urbana em relação ao ano anterior, onde estão os principais focos de alteração e qual classe apresentou maior variação. Hoje ele não tem tempo para exportar shapefiles, abrir no QGIS e calcular manualmente estatísticas por classe. Ele pensa que precisa transformar o mapa em números claros e comparáveis e que não pode perder tempo calculando manualmente.

No escritório, Ricardo dispõe de computador e internet. Sua formação em geografia o ajuda a interpretar mapas, mas a falta de uma visão consolidada no próprio sistema o obriga a usar ferramentas externas. Ele acessa a aba "Insights e Dashboard" após a segmentação: o sistema calcula proporção por classe, gera gráfico de pizza e gráfico de barras comparativo entre ano atual e anterior e destaca variações percentuais. Ao ativar o modo "Comparação Temporal", o sistema sobrepõe os mapas e destaca as áreas de mudança em cores contrastantes. O processamento é automático; os gráficos atualizam ao trocar filtros e um resumo interpretativo informa, por exemplo, que a classe Urbana apresentou crescimento de 12,4% em relação ao período anterior. Ricardo exporta um relatório em PDF com mapa, estatísticas, gráficos e resumo textual. O relatório fica pronto para entrega no prazo.

Ao mesmo tempo, Cláudia Torres precisa apresentar dados claros em uma reunião da Secretaria de Meio Ambiente. Ela não possui formação técnica em geoprocessamento e precisa de visualizações simples e compreensíveis. Ela pensa que precisa explicar tudo de forma simples para o conselho e que, se o mapa for muito técnico, ninguém vai entender. Ela depende do material que Ricardo ou o próprio sistema pode gerar: gráficos claros e resumo em linguagem não técnica, para apresentar os dados na reunião e apoiar decisões baseadas em evidências. O problema que ambos enfrentam é a dificuldade de interpretar resultados técnicos de segmentação para tomada de decisão estratégica quando não há estatísticas automáticas, comparação temporal integrada e relatório pronto na própria interface.

---

## 2. Conjunto de perguntas como resultado da análise

Perguntas de refinamento aplicadas ao tema do cenário, cobrindo os elementos da técnica (objetivo, ambiente, atores, planejamento, ação, evento, avaliação):

1. Quem pode ou deve obter estatísticas e insights a partir do mapa segmentado no GeoSegment? Em que momento do fluxo de trabalho isso ocorre?
2. Por que os atores precisam alcançar esse objetivo (relatório, apresentação, decisão)? Quais são as precondições (ex.: segmentação já realizada)?
3. De que informações ou conhecimentos os atores precisam para interpretar o resultado e tomar decisões (ex.: proporção por classe, comparação temporal)?
4. Quais informações são (ou deveriam ser) criadas, consumidas ou manipuladas pelo alcance do objetivo (mapa, gráficos, resumo textual, PDF)?
5. Em que situações o cenário ocorre: quando, onde e por quê (prazo do relatório, reunião na Secretaria)?
6. Que dispositivos e recursos (incluindo tempo) estão disponíveis para Ricardo e Cláudia alcançarem o objetivo?
7. Quais características dos atores os auxiliam ou atrapalham (formação técnica de Ricardo vs. não-técnica de Cláudia)?
8. De quem depende o alcance do objetivo? Quem fornece as informações necessárias (sistema, dados do ano anterior)?
9. Quem depende do resultado do objetivo? Quem consome as informações geradas e precisa ser notificado (ICMBio, Secretaria, conselho)?
10. Como os atores alcançam o objetivo atualmente? Como gostariam de fazê-lo (sem exportar para QGIS, sem planilhas)?
11. Que ações realizam e em que ordem? Há diferentes formas de realizá-las? Em que situações cada uma seria adotada?
12. Quais eventos são (ou deveriam ser) disparados pela realização das ações (atualização de gráficos, geração de PDF, destaque de áreas de mudança)?
13. Como os atores conseguem saber se uma ação foi concluída com sucesso (feedback visual, indicador de confiança, resumo interpretativo)?
14. Qual é o resultado do alcance do objetivo (relatório entregue, decisão tomada na reunião)? Em que pontos a interação pode ser mais eficiente?

---

## 3. Cenário refinado

Na primeira semana de fevereiro, Ricardo Mendes está no escritório do ICMBio em Petrópolis, com prazo curto para entregar um relatório sobre avanço urbano na APA [5]. Ele já realizou a segmentação automática de uma imagem aérea de alta resolução (30 cm/px) no GeoSegment e o sistema gerou o mapa segmentado corretamente [2]. Ricardo precisa responder perguntas estratégicas: qual porcentagem da área corresponde a vegetação nativa, se houve aumento de área urbana em relação ao ano anterior, onde estão os principais focos de alteração e qual classe apresentou maior variação [3]. Hoje ele não tem tempo para exportar shapefiles, abrir no QGIS e calcular manualmente estatísticas por classe [10]. Ele pensa: "Preciso transformar esse mapa em números claros e comparáveis. Não posso perder tempo calculando manualmente." [8]

Quem pode e deve obter essas estatísticas e insights a partir do mapa é o próprio analista, logo após a segmentação [1]. Para isso, ele depende de que o sistema ofereça proporções por classe e, idealmente, comparação com período anterior [8]. As informações que precisam ser criadas ou manipuladas são: distribuição percentual por classe, gráficos (pizza, barras), mapa de mudança e um resumo textual que traduza o resultado técnico em linguagem utilizável para relatórios [4]. No escritório, Ricardo dispõe de um computador conectado à internet e do tempo até a data de entrega do relatório [6]. Sua formação em geografia o ajuda a interpretar mapas, mas a falta de uma visão consolidada no próprio sistema o atrapalha e o obriga a usar ferramentas externas [7].

Ricardo acessa a aba "Insights e Dashboard" após a segmentação. O sistema calcula a proporção por classe, gera gráfico de pizza com a distribuição e gráfico de barras comparativo (ano atual vs. ano anterior), destacando variações percentuais [11]. Ao ativar o modo "Comparação Temporal", o sistema sobrepõe os mapas e destaca as áreas de mudança em cores contrastantes [12]. O processamento é automático e invisível ao usuário; os gráficos atualizam dinamicamente ao trocar filtros, e um indicador de confiança do modelo e um resumo interpretativo (por exemplo: "A classe Urbana apresentou crescimento de 12,4% em relação ao período anterior") permitem que ele saiba se o resultado é confiável e compreensível [13]. Ele exporta um relatório em PDF contendo mapa, estatísticas, gráficos e resumo textual [4]. O resultado do alcance do objetivo é o relatório entregue no prazo, com números e visualizações prontos para decisão [14].

Ao mesmo tempo, Cláudia Torres precisa apresentar dados claros em uma reunião da Secretaria de Meio Ambiente [5]. Ela não possui formação técnica em geoprocessamento e precisa de visualizações simples e compreensíveis [7]. Ela pensa: "Preciso explicar isso de forma simples para o conselho. Se o mapa for muito técnico, ninguém vai entender." Quem consome as informações geradas pelo sistema são tanto o ICMBio quanto gestores e o conselho; eles precisam de evidências visuais para tomar decisões, e em alguns fluxos seria desejável notificar envolvidos quando um relatório ou painel está pronto [9]. Cláudia depende do material que Ricardo (ou o próprio sistema) pode gerar: gráficos claros e resumo em linguagem não técnica [8]. O resultado esperado para ela é conseguir apresentar os dados na reunião e apoiar decisões baseadas em evidências [14]. Em que pontos a interação pode ser mais eficiente? Quando o sistema evita exportação manual, cálculo em planilhas e construção de gráficos externos, reduzindo carga cognitiva e permitindo que tanto o analista quanto a gestora passem do resultado técnico ao insight e à ação em minutos [14].

---

## Dashboard inicial (Histórico de uso e timeline)

**Título do cenário:** Monitoramento Temporal de Invasão na APA de Petrópolis

**Atores:** Ricardo Mendes (Analista Ambiental/Persona Primária) e Dra. Helena Silveira (Pesquisadora/Persona Primária).

---

## 1. Cenário inicial

Em uma manhã de trabalho na sede do ICMBio, Ricardo Mendes depara-se com um desafio crítico: um alerta de moradores aponta para uma construção possivelmente irregular em uma encosta de difícil acesso na APA de Petrópolis. Para confirmar a infração, ele precisa comparar o estado atual do terreno com registros passados. No fluxo tradicional, Ricardo teria que buscar arquivos TIFF pesados em diretórios locais e realizar uma comparação manual minuciosa em softwares como o QGIS, um processo que consumiria horas de esforço técnico e infraestrutura dedicada.


<<<<<<< HEAD
O objetivo de Ricardo é confirmar se houve conversão de Vegetação Densa em Urbano ou Solo Exposto e quantificar essa mudança para emitir um auto de infração. Como planejamento, ele decide utilizar o Dashboard Inicial da plataforma GeoSegment, visando agilizar a análise através da funcionalidade de Timeline e do histórico de uso.
Ao acessar a interface web, Ricardo realiza as seguintes ações: utiliza os filtros de localização e data para listar as inferências anteriores realizadas naquela coordenada específica. Ele localiza a segmentação de "Março de 2025" e a fixa na linha do tempo do sistema. Em seguida, faz o upload da imagem aérea capturada por drone naquela manhã e solicita o processamento.


Como evento e reação, o sistema, operando sob o modelo AIaaS (Inteligência Artificial como Serviço), processa a imagem via API utilizando o modelo V2 (DeepLabV3+). Em poucos segundos, o dashboard apresenta um gráfico comparativo e uma visualização lado a lado. Simultaneamente, a Dra. Helena Silveira, em seu laboratório, avalia os logs de desempenho da inferência para garantir que a métrica de acurácia (mIoU) se mantém estável, validando cientificamente a prova técnica gerada.
Na avaliação final da atividade, Ricardo interpreta os dados visuais: a cor Vermelha (Urbano) agora ocupa 15% de um polígono que antes era totalmente Verde Escuro (Vegetação Densa). Ele conclui que a invasão é real e recente. Ao exportar o relatório consolidado, Ricardo percebe como a interface agregou valor, transformando dados geoespaciais complexos em uma decisão de gestão territorial rápida, precisa e fundamentada.

---
=======
- Reduz carga cognitiva.
- Automatiza análise estatística e geração de gráficos e resumo.
- Traduz segmentação técnica em informação estratégica.
- Permite tomada de decisão em minutos.
- Conecta resultado técnico → insight → ação.

---

## Cenário 4 – Comparação temporal de resultados (Lucas Rebouças Silva)

**Funcionalidade (Tópico 01):** Comparação temporal de resultados.  
**Título:** Necessidade de comparar períodos (ex.: ano atual vs. anterior) para identificar mudanças e variações por classe.  
**Atores:** Ricardo Mendes, Felipe Antunes (consultor ambiental), Sistema GeoSegment.

**Cenário inicial:** Ricardo e Felipe precisam responder se houve aumento de área urbana ou alteração na cobertura vegetal em relação a um período anterior. Hoje isso exige exportar dados, abrir em outra ferramenta e calcular manualmente.

**Cenário refinado:** Após ter segmentações de dois períodos (ou acessar dados já processados), o usuário ativa o modo "Comparação Temporal" no Dashboard. O sistema sobrepõe os mapas e destaca as áreas de mudança em cores contrastantes; gráficos comparativos (ex.: barras ano atual vs. anterior) e variações percentuais por classe são exibidos. O usuário interpreta e pode incluir essa visão no relatório. Avaliação: comparação obtida sem sair da interface, em minutos.

**Problema evidenciado:** Trabalho manual de comparação em QGIS ou planilhas. **Valor da interface:** Comparação temporal integrada no Dashboard, com visualização e estatísticas automáticas (tela: Dashboard; ver Tópico 11).

---

## Cenário 5 – Dashboard inicial, Histórico e timeline (Victor Caldeira Iak)

**Funcionalidade (Tópico 01):** Dashboard inicial (Histórico de uso e timeline).  
**Título:** Necessidade de acessar rapidamente o histórico de processamentos e ter visão geral das atividades.  
**Atores:** Ricardo Mendes, Felipe Antunes, Sistema GeoSegment.

**Cenário inicial:** Analistas e consultores precisam retomar um processamento anterior, ver quando e o que foi processado, ou iniciar um novo fluxo a partir da visão geral. Sem histórico centralizado, perdem tempo buscando arquivos ou repetindo etapas.

**Cenário refinado:** O usuário acessa a Home do GeoSegment e vê o Dashboard inicial com histórico de uso e timeline (processamentos recentes, datas, áreas ou nomes associados). Pode clicar em um item para reabrir o resultado ou iniciar novo upload. O fluxo fica rastreável e o retorno a trabalhos anteriores é direto. Avaliação: histórico acessível e navegação clara entre passado e novo processamento.

**Problema evidenciado:** Falta de visão consolidada do que já foi processado e onde estão os resultados. **Valor da interface:** Home e Dashboard como ponto de partida com histórico e timeline (telas: Home inicial, Dashboard; ver Tópico 11).

---

## Rastreabilidade: Cenários × Funcionalidade × Responsável × Persona(s) × Tela(s)

| Cenário | Funcionalidade (Tópico 01) | Responsável | Persona(s) | Tela(s) principal(is) (Tópico 11) |
|---------|----------------------------|-------------|------------|-----------------------------------|
| 1 – Upload e segmentação | Segmentação de imagens | Vinicius Saidi Soares | Ricardo Mendes | Home, Upload de imagem |
| 2 – Seleção de modelo e validação técnica | Seleção de redes + informações técnicas | Gustavo Dias Vicentin | Dra. Helena Silveira | Upload, Seleção de rede, Dashboard |
| 3 – Insights e Dashboard | Geração de insights e dashboards | Deise Adriana Silva Araújo | Ricardo Mendes, Cláudia Torres | Dashboard |
| 4 – Comparação temporal | Comparação temporal de resultados | Lucas Rebouças Silva | Ricardo Mendes, Felipe Antunes | Dashboard |
| 5 – Histórico e timeline | Dashboard inicial (Histórico e timeline) | Victor Caldeira Iak | Ricardo Mendes, Felipe Antunes | Home inicial, Dashboard |
>>>>>>> 4a9fcea (Tópico 04: cinco cenários (um por funcionalidade), técnica de cenários explícita e tabela de rastreabilidade)
