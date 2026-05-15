# Avaliação Heurística de Usabilidade — Lucas Rebolças

> **Referência:** Heurísticas identificadas por Jakob Nielsen e Rolf Molich, traduzidas por Frederick van Amstel.  
> Molich, R., and Nielsen, J. (1990). *Improving a human-computer dialogue*, Communications of the ACM 33, 3 (March), 338–348.

---

| # | Título da Heurística | Descrição da Heurística | Problemas encontrados | Sugestões |
|:-:|---|---|---|---|
| 1 | Feedback | O sistema deve informar continuamente ao usuário sobre o que ele está fazendo. 10 segundos é o limite para manter a atenção do usuário focalizada no diálogo. | Durante o upload de imagens e execução das análises temporais, o sistema não apresenta barra de progresso ou estimativa de tempo restante, dificultando entender se o processamento ainda está ocorrendo. | Adicionar barra de progresso, animações de carregamento e mensagens indicando processamento e conclusão das análises. |
| 2 | Falar a linguagem do usuário | A terminologia deve ser baseada na linguagem do usuário e não orientada ao sistema. As informações devem ser organizadas conforme o modelo mental do usuário. | Os modelos “U-Net” e “DeepLabV3+” aparecem sem explicação simplificada, dificultando entendimento de usuários sem conhecimento técnico. | Inserir descrições resumidas, exemplos de aplicação e tooltips explicando os modelos disponíveis. |
| 3 | Saídas claramente demarcadas | O usuário controla o sistema; ele pode, a qualquer momento, abortar uma tarefa ou desfazer uma operação e retornar ao estado anterior. | O sistema não possui botão claro para cancelar upload ou reiniciar rapidamente uma nova comparação após análise concluída. | Adicionar ações rápidas como “Cancelar Upload”, “Nova Comparação” e “Voltar para Análise”. |
| 4 | Consistência | Um mesmo comando ou ação deve ter sempre o mesmo efeito. A mesma operação deve ser apresentada na mesma localização e formatada da mesma maneira para facilitar o reconhecimento. | Alguns espaçamentos e tamanhos de textos variam entre cards e telas do sistema, reduzindo padronização visual completa. | Padronizar tipografia, tamanhos de componentes e espaçamentos utilizando um design system consistente. |
| 5 | Prevenir erros | Evitar situações de erro. Conhecer as situações que mais provocam erros e modificar a interface para que estes erros não ocorram. | A tela de upload não informa claramente tamanho máximo permitido antes do envio do arquivo. | Exibir mensagens preventivas com formatos aceitos, limite de tamanho e restrições antes do envio da imagem. |
| 6 | Minimizar a sobrecarga de memória do usuário | O sistema deve mostrar os elementos de diálogo e permitir que o usuário faça suas escolhas sem necessidade de lembrar comandos específicos. | Os modelos são apresentados apenas por nomes técnicos, exigindo que o usuário memorize diferenças entre eles. | Adicionar descrições visuais e explicações rápidas sobre cada modelo para facilitar reconhecimento imediato. |
| 7 | Atalhos | Para usuários experientes executarem operações mais rapidamente. Abreviações, teclas de função, duplo clique e funções de retorno auxiliam na navegação. | O histórico não possui filtros ou pesquisa rápida para localizar análises específicas. | Implementar filtros por data, pesquisa por nome do projeto e ordenação personalizada no histórico. |
| 8 | Diálogos simples e naturais | Deve-se apresentar exatamente a informação que o usuário precisa no momento, nem mais nem menos. | A tela de comparação temporal apresenta muitos gráficos e métricas simultaneamente, causando sobrecarga visual. | Organizar gráficos em abas, seções recolhíveis ou agrupamentos para reduzir excesso visual. |
| 9 | Boas mensagens de erro | Linguagem clara e sem códigos. Devem ajudar o usuário a entender e resolver o problema sem intimidá-lo. | As mensagens de erro utilizam alertas genéricos do navegador sem orientação detalhada para solução do problema. | Substituir alertas do navegador por mensagens visuais integradas à interface, com explicações e ações de correção. |
| 10 | Ajuda e documentação | O ideal é que o software seja intuitivo, mas caso necessário a ajuda deve estar facilmente acessível online. | O sistema não possui tutorial inicial ou ajuda contextual para usuários iniciantes compreenderem funcionalidades avançadas. | Adicionar onboarding inicial, documentação simplificada e ajuda contextual sobre funcionalidades e modelos disponíveis. |

---

**Arquivo base utilizado:** :contentReference[oaicite:0]{index=0}
