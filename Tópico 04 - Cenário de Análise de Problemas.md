# Tópico 4 – Cenário de Análise de Problemas

Cada uma das **cinco grandes funcionalidades** do sistema (Tópico 01) possui um cenário de análise de problemas, vinculado ao integrante responsável e à(s) persona(s) correspondente(s). Em cada cenário utilizam-se os **elementos da técnica de cenários**: **objetivo** (o que se quer alcançar), **ambiente** (onde e quando ocorre), **atores** (quem participa), **planejamento** (ordem e condições), **ação** (o que o usuário faz), **evento** (o que o sistema faz ou responde) e **avaliação** (como se verifica o sucesso e o resultado).

---

## Cenário 1 – Upload e segmentação de imagens (Vinicius Saidi Soares)

**Funcionalidade (Tópico 01):** Segmentação de imagens – upload e processamento.  
**Título:** Necessidade de carregar imagens de forma rápida e confiável para segmentação semântica.  
**Atores:** Ricardo Mendes (analista ambiental do ICMBio), Sistema GeoSegment.

**Cenário inicial:** Ricardo precisa enviar uma imagem aérea (ex.: .tiff ou .png) da APA de Petrópolis para obter o mapa segmentado. Hoje depende de ferramentas locais ou processos manuais. Objetivo: reduzir tempo e garantir que o formato e o tamanho do arquivo sejam aceitos, com feedback claro de progresso.
## 2. Conjunto de perguntas como resultado da análise

1. Quem precisa ou deve fazer o upload de imagens no GeoSegment? Em que momento do fluxo isso ocorre?
2. Por que os atores precisam que o upload seja rápido e confiável? Quais são as precondições (ex.: tamanho, formato do arquivo)?
3. Que informações o usuário precisa durante o upload para sentir-se seguro (ex.: barra de progresso, validação de formato)?
4. Quais eventos são disparados pelo sistema durante a ação (upload iniciado, falha de validação, conclusão)?
5. Como os usuários sabem se o upload foi bem‑sucedido (feedback visual, mensagem de confirmação)?
6. Que dispositivos e recursos estão disponíveis para o upload (banda de internet, tipos de arquivo aceitos)?
7. Há situações em que o upload falha? Como o sistema deve reagir?
8. De quem depende o sucesso do upload (provedor de serviço, rede)?
9. Quem consome o resultado do upload (o próprio usuário, a rede neural no backend)?
10. Como o usuário alcança esse objetivo hoje e como gostaria de fazê‑lo (sem ferramentas locais)?
 
**Cenário refinado:** Ricardo acessa a Home do GeoSegment e segue para a tela de Upload. Seleciona o arquivo; o sistema informa o status (upload em andamento, validação). Após o upload, pode escolher a rede (Cenário 2) e disparar a segmentação. O sistema exibe indicador de processamento e, ao concluir, leva à visualização (original vs. segmentado). Avaliação: upload concluído sem erro, resultado visível em tempo hábil. _O passo em que o sistema informa o status e valida o arquivo responde às perguntas 3 e 4; a conclusão sem erro atende à pergunta 5._

**Problema evidenciado:** Dependência de softwares locais; falta de feedback durante o processamento. **Valor da interface:** Acesso web, upload direto, visibilidade do status e resultado integrado (telas: Home, Upload de imagem; ver Tópico 11).

---

## Cenário 2 – Seleção de rede neural e validação técnica (Gustavo Dias Vicentin)

**Funcionalidade (Tópico 01):** Seleção de redes neurais e informações técnicas.  
**Título:** Pesquisadora precisa escolher o modelo e acessar métricas para validação científica.  
**Atores:** Dra. Helena Silveira (pesquisadora), Sistema GeoSegment.

**Cenário inicial:** Helena precisa comparar as arquiteturas (V0, V1, V2) e justificar o uso do modelo em publicação. Necessita saber qual rede está em uso, ver parâmetros e métricas (ex.: mIoU, IoU por classe) sem configurar ambiente local.
## 2. Conjunto de perguntas como resultado da análise

1. Quem são os atores que precisam selecionar a rede e por quê? Em que ponto do fluxo de trabalho isso ocorre?
2. Quais critérios os atores usam para decidir entre as arquiteturas disponíveis (V0, V1, V2)?
3. Que informações técnicas precisam estar visíveis para justificar a escolha (mIoU, IoU por classe, parâmetros)?
4. Como o sistema deve apresentar essas informações (tabela, gráfico, texto explicativo)?
5. Quais eventos o sistema deve disparar ao mudar de modelo (atualização de métricas, reinício de processamento)?
6. Como os atores contam com feedback para saber se a seleção foi aplicada corretamente?
7. Quais recursos estão disponíveis para análise (documentação, exemplos de métricas anteriores)?
8. De quem depende a disponibilidade da rede (equipe de infraestrutura, provedor de IA)?
9. Quem consome esse resultado técnico (pesquisadores, relatórios, publicações)?
10. Como os atores realizam essa validação hoje e como gostariam de fazê‑lo na nova interface?
 
**Cenário refinado:** Após o upload (Cenário 1), Helena acessa a tela de Seleção de rede. Escolhe o modelo (ex.: DeepLabV3+ / V2), visualiza informações técnicas (rede em uso, métricas de referência). Dispara a segmentação e analisa o resultado no Dashboard, com foco em classes desbalanceadas e refinamento de bordas. Avaliação: decisão embasada em dados técnicos visíveis na própria interface. _A exibição de métricas e a escolha do modelo respondem às perguntas 2, 3 e 4; a avaliação técnica atende à pergunta 6._

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

_A geração automática dos gráficos e do resumo textual responde às perguntas 1–4; a exportação para PDF cobre as perguntas 10 e 14; a referência ao prazo e à reunião atende 5 e 9; e o indicador de confiança lida com a pergunta 13._

Quem pode e deve obter essas estatísticas e insights a partir do mapa é o próprio analista, logo após a segmentação [1]. Para isso, ele depende de que o sistema ofereça proporções por classe e, idealmente, comparação com período anterior [8]. As informações que precisam ser criadas ou manipuladas são: distribuição percentual por classe, gráficos (pizza, barras), mapa de mudança e um resumo textual que traduza o resultado técnico em linguagem utilizável para relatórios [4]. No escritório, Ricardo dispõe de um computador conectado à internet e do tempo até a data de entrega do relatório [6]. Sua formação em geografia o ajuda a interpretar mapas, mas a falta de uma visão consolidada no próprio sistema o atrapalha e o obriga a usar ferramentas externas [7].

Ricardo acessa a aba "Insights e Dashboard" após a segmentação. O sistema calcula a proporção por classe, gera gráfico de pizza com a distribuição e gráfico de barras comparativo (ano atual vs. ano anterior), destacando variações percentuais [11]. Ao ativar o modo "Comparação Temporal", o sistema sobrepõe os mapas e destaca as áreas de mudança em cores contrastantes [12]. O processamento é automático e invisível ao usuário; os gráficos atualizam dinamicamente ao trocar filtros, e um indicador de confiança do modelo e um resumo interpretativo (por exemplo: "A classe Urbana apresentou crescimento de 12,4% em relação ao período anterior") permitem que ele saiba se o resultado é confiável e compreensível [13]. Ele exporta um relatório em PDF contendo mapa, estatísticas, gráficos e resumo textual [4]. O resultado do alcance do objetivo é o relatório entregue no prazo, com números e visualizações prontos para decisão [14].

Ao mesmo tempo, Cláudia Torres precisa apresentar dados claros em uma reunião da Secretaria de Meio Ambiente [5]. Ela não possui formação técnica em geoprocessamento e precisa de visualizações simples e compreensíveis [7]. Ela pensa: "Preciso explicar isso de forma simples para o conselho. Se o mapa for muito técnico, ninguém vai entender." Quem consome as informações geradas pelo sistema são tanto o ICMBio quanto gestores e o conselho; eles precisam de evidências visuais para tomar decisões, e em alguns fluxos seria desejável notificar envolvidos quando um relatório ou painel está pronto [9]. Cláudia depende do material que Ricardo (ou o próprio sistema) pode gerar: gráficos claros e resumo em linguagem não técnica [8]. O resultado esperado para ela é conseguir apresentar os dados na reunião e apoiar decisões baseadas em evidências [14]. Em que pontos a interação pode ser mais eficiente? Quando o sistema evita exportação manual, cálculo em planilhas e construção de gráficos externos, reduzindo carga cognitiva e permitindo que tanto o analista quanto a gestora passem do resultado técnico ao insight e à ação em minutos [14].

 
## Cenário 4 – Comparação temporal de resultados (Lucas Rebouças Silva)

**Funcionalidade (Tópico 01):** Comparação temporal de resultados.  
**Título:** Necessidade de comparar períodos (ex.: ano atual vs. anterior) para identificar mudanças e variações por classe.  
**Atores:** Ricardo Mendes, Felipe Antunes (consultor ambiental), Sistema GeoSegment.

**Cenário inicial:** Ricardo e Felipe precisam responder se houve aumento de área urbana ou alteração na cobertura vegetal em relação a um período anterior. Hoje isso exige exportar dados, abrir em outra ferramenta e calcular manualmente – um processo semelhante ao que leva Helena a procurar métricas no Cenário 3, mas aqui a dificuldade está na comparação entre arquivos processados.

**Cenário refinado:** Após ter segmentações de dois períodos (ou acessar dados já processados), o usuário ativa o modo "Comparação Temporal" no Dashboard (mesma aba utilizada em Cenário 3). O sistema sobrepõe os mapas e destaca as áreas de mudança em cores contrastantes; gráficos comparativos (ex.: barras ano atual vs. anterior) e variações percentuais por classe são exibidos. O usuário interpreta e pode incluir essa visão no relatório ou painel de insights. Avaliação: comparação obtida sem sair da interface, em minutos, com feedback visual imediato sobre a confiabilidade dos dados.

_A sobreposição dos mapas e os gráficos comparativos respondem às perguntas 3 e 4; a indicação de variação percentual atende 5 e 6; a rapidez de obtenção resolve 10._

**Problema evidenciado:** Trabalho manual de comparação em QGIS ou planilhas. **Valor da interface:** Comparação temporal integrada no Dashboard, com visualização e estatísticas automáticas (tela: Dashboard; ver Tópico 11).

## 2. Conjunto de perguntas como resultado da análise

1. Quem precisa comparar períodos e com que frequência? Em que fase do uso do sistema essa comparação ocorre?
2. Por que a comparação temporal é importante para os atores (monitoramento de mudanças, relatórios)?
3. Que tipos de mudanças devem ser destacados (aumento urbano, perda de vegetação)?
4. Como as informações devem ser apresentadas (mapa sobreposto, gráfico comparativo)?
5. Quais eventos o sistema deve disparar ao ativar o modo de comparação (atualização de mapas, cálculo de variação)?
6. Como o usuário sabe que a comparação está correta (feedback visual, mensagem de confiança)?
7. Que dados históricos são necessários e como são acessados?
8. De quem depende o histórico (banco de dados, servidores)?
9. Quem consome o resultado da comparação (analistas, relatórios, decisões)?
10. Como esse objetivo é alcançado hoje e como seria ideal na interface?

---

## Cenário 5 – Dashboard inicial, Histórico e timeline (Victor Caldeira Iak)

**Funcionalidade (Tópico 01):** Dashboard inicial (Histórico de uso e timeline).  
**Título:** Necessidade de acessar rapidamente o histórico de processamentos e ter visão geral das atividades.  
**Atores:** Ricardo Mendes, Felipe Antunes, Sistema GeoSegment.

**Cenário inicial:** Analistas e consultores precisam retomar um processamento anterior, ver quando e o que foi processado, ou iniciar um novo fluxo a partir da visão geral. Sem histórico centralizado, perdem tempo buscando arquivos ou repetindo etapas. O problema espelha a falta de rastreabilidade que no Cenário 3 obrigaria Ricardo a recalcular manualmente estatísticas antigas.

**Cenário refinado:** O usuário acessa a Home do GeoSegment e vê o Dashboard inicial com histórico de uso e timeline (processamentos recentes, datas, áreas ou nomes associados). Pode clicar em um item para reabrir o resultado ou iniciar novo upload. O fluxo fica rastreável e o retorno a trabalhos anteriores é direto, facilitando também a revisão de painéis de insights previamente gerados. Avaliação: histórico acessível e navegação clara entre passado e novo processamento.
_A descrição da Home com histórico e timeline trata as perguntas 1–3; a navegação direta responde 4 e 5; e a facilidade de retorno ao fluxo atende 9._

**Problema evidenciado:** Falta de visão consolidada do que já foi processado e onde estão os resultados. **Valor da interface:** Home e Dashboard como ponto de partida com histórico e timeline (telas: Home inicial, Dashboard; ver Tópico 11).

## 2. Conjunto de perguntas como resultado da análise

1. Quem utiliza o histórico de uso e por quê? Em quais situações eles retornam a processamentos anteriores?
2. Que informações devem constar no histórico (data, área, tipo de processamento)?
3. Como deve funcionar a linha do tempo (filtros, fixação de itens)?
4. Que eventos o sistema dispara ao reabrir um processamento (carregamento de resultados, navegação)?
5. Como os usuários sabem que estão acessando o item correto (rótulos claros, miniaturas)?
6. Quais dispositivos e recursos estão disponíveis para consultar o histórico?
7. De quem depende a manutenção desse histórico (backend, banco de dados)?
8. Quem consome esses registros (analistas, consultores)?
9. Como o histórico é gerenciado atualmente e como poderia ser melhorado?

---


## Rastreabilidade: Cenários × Funcionalidade × Responsável × Persona(s) × Tela(s)

| Cenário | Funcionalidade (Tópico 01) | Responsável | Persona(s) | Tela(s) principal(is) (Tópico 11) |
|---------|----------------------------|-------------|------------|-----------------------------------|
| 1 – Upload e segmentação | Segmentação de imagens | Vinicius Saidi Soares | Ricardo Mendes | Home, Upload de imagem |
| 2 – Seleção de modelo e validação técnica | Seleção de redes + informações técnicas | Gustavo Dias Vicentin | Dra. Helena Silveira | Upload, Seleção de rede, Dashboard |
| 3 – Insights e Dashboard | Geração de insights e dashboards | Deise Adriana Silva Araújo | Ricardo Mendes, Cláudia Torres | Dashboard |
| 4 – Comparação temporal | Comparação temporal de resultados | Lucas Rebouças Silva | Ricardo Mendes, Felipe Antunes | Dashboard |
| 5 – Histórico e timeline | Dashboard inicial (Histórico e timeline) | Victor Caldeira Iak | Ricardo Mendes, Felipe Antunes | Home inicial, Dashboard |
<!-- merge artifact removed -->
