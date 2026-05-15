# Avaliação Heurística de Usabilidade — Deise Araujo

> **Referência:** Heurísticas identificadas por Jakob Nielsen e Rolf Molich, traduzidas por Frederick van Amstel.  
> Molich, R., and Nielsen, J. (1990). *Improving a human-computer dialogue*, Communications of the ACM 33, 3 (March), 338–348.

---

| # | Título da Heurística | Descrição da Heurística | Problemas encontrados | Sugestões |
|:-:|---|---|---|---|
| 1 | Feedback | O sistema deve informar continuamente ao usuário sobre o que ele está fazendo. 10 segundos é o limite para manter a atenção do usuário focalizada no diálogo. | Durante o upload de imagens e execução das análises temporais, o sistema não apresenta barra de progresso ou estimativa de tempo restante, dificultando entender se o processamento ainda está ocorrendo. | Adicionar barra de progresso, spinner e mensagens visuais indicando carregamento, processamento e conclusão das análises. |
| 2 | Falar a linguagem do usuário | A terminologia deve ser baseada na linguagem do usuário e não orientada ao sistema. As informações devem ser organizadas conforme o modelo mental do usuário. | Os modelos “U-Net” e “DeepLabV3+” aparecem sem explicação simplificada, dificultando entendimento de usuários sem conhecimento técnico. | Inserir descrições simplificadas, exemplos práticos e tooltips explicando a função de cada modelo disponível. |
| 3 | Saídas claramente demarcadas | O usuário controla o sistema; ele pode, a qualquer momento, abortar uma tarefa ou desfazer uma operação e retornar ao estado anterior. | O sistema não possui botão claro para cancelar upload ou reiniciar rapidamente uma nova comparação após análise concluída. | Adicionar botões como “Cancelar Upload”, “Nova Comparação” e “Refazer Análise” após o processamento. |
| 4 | Consistência | Um mesmo comando ou ação deve ter sempre o mesmo efeito. A mesma operação deve ser apresentada na mesma localização e formatada da mesma maneira para facilitar o reconhecimento. | Alguns espaçamentos e tamanhos de textos variam entre cards e telas do sistema, reduzindo a padronização visual completa. | Padronizar tipografia, espaçamentos e dimensões dos componentes seguindo um guia visual único para toda aplicação. |
| 5 | Prevenir erros | Evitar situações de erro. Conhecer as situações que mais provocam erros e modificar a interface para que estes erros não ocorram. | A tela de upload não informa claramente tamanho máximo permitido antes do envio do arquivo. | Exibir mensagens preventivas informando formatos suportados, tamanho máximo permitido e possíveis restrições do upload. |
| 6 | Minimizar a sobrecarga de memória do usuário | O sistema deve mostrar os elementos de diálogo e permitir que o usuário faça suas escolhas sem necessidade de lembrar comandos específicos. | Os modelos são apresentados apenas por nomes técnicos, exigindo que o usuário memorize diferenças entre eles. | Adicionar descrições rápidas, exemplos visuais e explicações resumidas para facilitar reconhecimento imediato dos modelos. |
| 7 | Atalhos | Para usuários experientes executarem operações mais rapidamente. Abreviações, teclas de função, duplo clique e funções de retorno auxiliam na navegação. | O histórico não possui filtros ou pesquisa rápida para localizar análises específicas. | Implementar busca por nome, filtros por data e modelo utilizado, além de ordenação personalizada no histórico. |
| 8 | Diálogos simples e naturais | Deve-se apresentar exatamente a informação que o usuário precisa no momento, nem mais nem menos. | A tela de comparação temporal apresenta muitos gráficos e métricas simultaneamente, causando sobrecarga visual. | Organizar informações em abas, categorias ou seções recolhíveis para melhorar leitura e reduzir excesso visual. |
| 9 | Boas mensagens de erro | Linguagem clara e sem códigos. Devem ajudar o usuário a entender e resolver o problema sem intimidá-lo. | As mensagens de erro utilizam alertas genéricos do navegador sem orientação detalhada para solução do problema. | Substituir alertas nativos por mensagens visuais integradas à interface com explicações claras e sugestões de correção. |
| 10 | Ajuda e documentação | O ideal é que o software seja intuitivo, mas caso necessário a ajuda deve estar facilmente acessível online. | O sistema não possui tutorial inicial ou ajuda contextual para usuários iniciantes compreenderem funcionalidades avançadas. | Adicionar onboarding inicial, tooltips explicativos e documentação simplificada sobre funcionalidades e modelos disponíveis. |

---

**Arquivo base utilizado:** :contentReference[oaicite:0]{index=0}
