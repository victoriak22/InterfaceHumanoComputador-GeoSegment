# Tópico 4 – Cenário de Análise de Problemas

## Geração de Insights e Painéis para Apoio à Decisão Territorial

**Título do cenário:** Dificuldade na interpretação de resultados técnicos de segmentação para tomada de decisão estratégica.

**Atores:** Ricardo Mendes (analista ambiental do ICMBio), Cláudia Torres (gestora de políticas públicas), Sistema GeoSegment (interface web com dashboards).

---

## 1. Cenário inicial (antes do refinamento)

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

## 3. Cenário refinado (depois do refinamento)

Na primeira semana de fevereiro, Ricardo Mendes está no escritório do ICMBio em Petrópolis, com prazo curto para entregar um relatório sobre avanço urbano na APA [5]. Ele já realizou a segmentação automática de uma imagem aérea de alta resolução (30 cm/px) no GeoSegment e o sistema gerou o mapa segmentado corretamente [2]. Ricardo precisa responder perguntas estratégicas: qual porcentagem da área corresponde a vegetação nativa, se houve aumento de área urbana em relação ao ano anterior, onde estão os principais focos de alteração e qual classe apresentou maior variação [3]. Hoje ele não tem tempo para exportar shapefiles, abrir no QGIS e calcular manualmente estatísticas por classe [10]. Ele pensa: "Preciso transformar esse mapa em números claros e comparáveis. Não posso perder tempo calculando manualmente." [8]

Quem pode e deve obter essas estatísticas e insights a partir do mapa é o próprio analista, logo após a segmentação [1]. Para isso, ele depende de que o sistema ofereça proporções por classe e, idealmente, comparação com período anterior [8]. As informações que precisam ser criadas ou manipuladas são: distribuição percentual por classe, gráficos (pizza, barras), mapa de mudança e um resumo textual que traduza o resultado técnico em linguagem utilizável para relatórios [4]. No escritório, Ricardo dispõe de um computador conectado à internet e do tempo até a data de entrega do relatório [6]. Sua formação em geografia o ajuda a interpretar mapas, mas a falta de uma visão consolidada no próprio sistema o atrapalha e o obriga a usar ferramentas externas [7].

Ricardo acessa a aba "Insights e Dashboard" após a segmentação. O sistema calcula a proporção por classe, gera gráfico de pizza com a distribuição e gráfico de barras comparativo (ano atual vs. ano anterior), destacando variações percentuais [11]. Ao ativar o modo "Comparação Temporal", o sistema sobrepõe os mapas e destaca as áreas de mudança em cores contrastantes [12]. O processamento é automático e invisível ao usuário; os gráficos atualizam dinamicamente ao trocar filtros, e um indicador de confiança do modelo e um resumo interpretativo (por exemplo: "A classe Urbana apresentou crescimento de 12,4% em relação ao período anterior") permitem que ele saiba se o resultado é confiável e compreensível [13]. Ele exporta um relatório em PDF contendo mapa, estatísticas, gráficos e resumo textual [4]. O resultado do alcance do objetivo é o relatório entregue no prazo, com números e visualizações prontos para decisão [14].

Ao mesmo tempo, Cláudia Torres precisa apresentar dados claros em uma reunião da Secretaria de Meio Ambiente [5]. Ela não possui formação técnica em geoprocessamento e precisa de visualizações simples e compreensíveis [7]. Ela pensa: "Preciso explicar isso de forma simples para o conselho. Se o mapa for muito técnico, ninguém vai entender." Quem consome as informações geradas pelo sistema são tanto o ICMBio quanto gestores e o conselho; eles precisam de evidências visuais para tomar decisões, e em alguns fluxos seria desejável notificar envolvidos quando um relatório ou painel está pronto [9]. Cláudia depende do material que Ricardo (ou o próprio sistema) pode gerar: gráficos claros e resumo em linguagem não técnica [8]. O resultado esperado para ela é conseguir apresentar os dados na reunião e apoiar decisões baseadas em evidências [14]. Em que pontos a interação pode ser mais eficiente? Quando o sistema evita exportação manual, cálculo em planilhas e construção de gráficos externos, reduzindo carga cognitiva e permitindo que tanto o analista quanto a gestora passem do resultado técnico ao insight e à ação em minutos [14].

---

## Passo a passo (referência à técnica)

- Construiu-se o **cenário inicial** (antes do refinamento) como narrativa em texto, com elementos do cenário de problema.
- Definidas as **questões de refinamento** aplicadas ao tema do cenário (itens 1 a 14), cobrindo objetivo, ambiente, atores, planejamento, ação, evento e avaliação.
- Construiu-se o **cenário refinado** (depois do refinamento): mesma narrativa enriquecida, com cada questão localizada onde é respondida e sinalizada com o número entre colchetes [n].

---

## Problema evidenciado (síntese)

- Exportação manual de dados para QGIS ou planilhas.
- Cálculo manual de estatísticas por classe.
- Construção de gráficos em ferramentas externas.
- Interpretação de números brutos sem apoio visual e sem resumo interpretativo.
- Gasto excessivo de tempo em tarefas operacionais em vez de análise e decisão.

## Como a interface agrega valor (síntese)

- Reduz carga cognitiva.
- Automatiza análise estatística e geração de gráficos e resumo.
- Traduz segmentação técnica em informação estratégica.
- Permite tomada de decisão em minutos.
- Conecta resultado técnico → insight → ação.
