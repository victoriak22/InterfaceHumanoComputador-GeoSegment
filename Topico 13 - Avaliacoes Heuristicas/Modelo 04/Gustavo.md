# Avaliação Heurística de Usabilidade — Gustavo Dias Vicentin

> **Referência:** Heurísticas identificadas por Jakob Nielsen e Rolf Molich, traduzidas por Frederick van Amstel.  
> Molich, R., and Nielsen, J. (1990). *Improving a human-computer dialogue*, Communications of the ACM 33, 3 (March), 338–348.

---

| # | Título da Heurística | Descrição da Heurística | Problemas encontrados | Sugestões |
|:-:|---|---|---|---|
| 1 | Feedback | O sistema deve informar continuamente ao usuário sobre o que ele está fazendo. 10 segundos é o limite para manter a atenção do usuário focalizada no diálogo. | O histórico e algumas análises não apresentam indicador de carregamento, fazendo o usuário acreditar que o sistema travou durante o processamento das informações. | Adicionar skeleton loading, barras de progresso e mensagens visuais indicando carregamento e conclusão das análises. |
| 2 | Falar a linguagem do usuário | A terminologia deve ser baseada na linguagem do usuário e não orientada ao sistema. As informações devem ser organizadas conforme o modelo mental do usuário. | Algumas métricas ambientais e nomes técnicos utilizados nos modelos dificultam entendimento para usuários sem experiência em geoprocessamento ou inteligência artificial. | Adicionar descrições simplificadas, exemplos visuais e tooltips explicando termos técnicos e métricas apresentadas. |
| 3 | Saídas claramente demarcadas | O usuário controla o sistema; ele pode, a qualquer momento, abortar uma tarefa ou desfazer uma operação e retornar ao estado anterior. | O sistema não oferece opção rápida para retornar às configurações anteriores após finalizar uma comparação temporal. | Inserir botões como “Refazer Comparação”, “Editar Configurações” e “Nova Análise” após conclusão do processamento. |
| 4 | Consistência | Um mesmo comando ou ação deve ter sempre o mesmo efeito. A mesma operação deve ser apresentada na mesma localização e formatada da mesma maneira para facilitar o reconhecimento. | Alguns botões possuem tamanhos e alinhamentos diferentes entre telas, reduzindo a padronização visual da interface. | Padronizar dimensões, estilos de botões e espaçamentos utilizando um guia visual único para toda aplicação. |
| 5 | Prevenir erros | Evitar situações de erro. Conhecer as situações que mais provocam erros e modificar a interface para que estes erros não ocorram. | O sistema não apresenta mensagens preventivas claras explicando formatos aceitos e limitações antes do envio das imagens. | Exibir formatos compatíveis, tamanho máximo permitido e mensagens preventivas diretamente na área de upload. |
| 6 | Minimizar a sobrecarga de memória do usuário | O sistema deve mostrar os elementos de diálogo e permitir que o usuário faça suas escolhas sem necessidade de lembrar comandos específicos. | Os modelos disponíveis não possuem exemplos visuais ou descrições rápidas, dificultando reconhecimento imediato de suas diferenças. | Adicionar miniaturas, descrições resumidas e exemplos de aplicação para cada modelo disponível. |
| 7 | Atalhos | Para usuários experientes executarem operações mais rapidamente. Abreviações, teclas de função, duplo clique e funções de retorno auxiliam na navegação. | Não existe campo de busca ou filtros rápidos para localizar análises antigas no histórico do sistema. | Implementar pesquisa por nome, filtros por data, modelo utilizado e ordenação personalizada no histórico. |
| 8 | Diálogos simples e naturais | Deve-se apresentar exatamente a informação que o usuário precisa no momento, nem mais nem menos. | A tela de comparação apresenta muitas métricas e gráficos simultaneamente, dificultando leitura rápida dos resultados. | Organizar resultados em abas, categorias ou seções recolhíveis para reduzir sobrecarga visual. |
| 9 | Boas mensagens de erro | Linguagem clara e sem códigos. Devem ajudar o usuário a entender e resolver o problema sem intimidá-lo. | As mensagens de erro não apresentam botão “Tentar novamente” nem orientações claras para recuperação das operações falhadas. | Criar mensagens de erro amigáveis com explicações objetivas, botão de repetição da ação e sugestões de solução. |
| 10 | Ajuda e documentação | O ideal é que o software seja intuitivo, mas caso necessário a ajuda deve estar facilmente acessível online. | Os modelos de IA utilizados não possuem documentação simples explicando funcionalidades, vantagens e aplicações práticas. | Adicionar seção de ajuda contextual, onboarding inicial e documentação simplificada sobre cada modelo disponível. |

---

**Arquivo base utilizado:** :contentReference[oaicite:0]{index=0}
