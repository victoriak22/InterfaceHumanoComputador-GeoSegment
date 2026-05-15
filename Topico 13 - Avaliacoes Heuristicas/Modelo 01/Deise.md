# Heurística 1 — Visibilidade do Status do Sistema

> **Definição:** O sistema deve sempre manter os usuários informados sobre o que está acontecendo, através de feedback apropriado em um tempo razoável.
>
> **Verificação:** Os usuários são mantidos informados sobre o progresso do sistema com apropriado feedback em um tempo razoável?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
O menu lateral destaca em verde a seção ativa, mantendo o usuário sempre orientado sobre onde está no sistema. Os cards de segmentações recentes exibem nome do projeto, data e badge com o modelo utilizado, fornecendo visibilidade imediata do estado das análises disponíveis.

**Exemplo da aplicação:** menu lateral com item "Home" destacado em verde e cards com informações de status visíveis. 

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" /> 

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O painel lateral exibe o status "Aguardando upload", informando o estado atual do sistema. No entanto, durante o carregamento do arquivo não há barra de progresso ou indicador visual contínuo, deixando o usuário sem feedback enquanto a imagem é enviada.

**Boa prática sugerida:**  
Adicionar barra de progresso visível na área de upload durante o carregamento do arquivo, com percentual ou animação indicando que o sistema está processando.

**Exemplo da aplicação:** painel direito com status "Aguardando upload" sem indicador de progresso durante o envio.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
O modelo selecionado é destacado visualmente com borda verde, deixando claro ao usuário qual opção está ativa. O botão de processamento atualiza seu rótulo dinamicamente para refletir o modelo escolhido (ex: "Processar com DeepLabV3+"), reforçando o feedback de estado de forma clara e imediata.

**Exemplo da aplicação:** card do modelo DeepLabV3+ com borda verde de seleção ativa e botão "Processar com DeepLabV3+" refletindo a escolha.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os resultados são apresentados com indicadores visuais claros: cards coloridos com percentuais de mudança (+12,4% Expansão Urbana, -7,6% Desmatamento), período de tempo analisado, área total e área alterada. O usuário tem visibilidade completa do que foi processado e dos resultados gerados. A tela de insights complementa o feedback visual exibindo gráficos comparativos, distribuição do uso do solo e resumo textual das mudanças detectadas automaticamente.

**Exemplo da aplicação:** cards de "Mudanças Detectadas" com percentuais, indicadores coloridos e métricas de área e período.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
Os cards exibem claramente as informações de cada análise: miniatura da imagem, nome do projeto, data de criação e badge com o modelo utilizado. O menu lateral destaca "Histórico" como seção ativa, orientando o usuário sobre onde está no sistema.

**Exemplo da aplicação:** grid de cards com miniaturas, nomes, datas e badges de modelo; menu lateral com "Histórico" em verde.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Parcialmente Atendida

**Justificativa:**  
O menu lateral destaca "Sobre" como seção ativa. No entanto, para uma página com múltiplas seções (Propósito, Funcionalidades, Tecnologia), não há indicador de progresso de scroll ou âncora ativa que oriente o usuário sobre em qual parte do conteúdo está posicionado.

**Boa prática sugerida:**  
Adicionar navegação interna com âncoras destacadas e indicador da seção ativa conforme o usuário rola a página, similar a um sumário lateral fixo.

**Exemplo da aplicação:** menu lateral com "Sobre" destacado, sem indicador de seção ativa dentro da própria página.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 2 — Correspondência entre o Sistema e o Mundo Real

> **Definição:** O sistema deve falar a linguagem do usuário, utilizando palavras, conceitos e convenções familiares, seguindo a lógica do mundo real.
>
> **Verificação:** Os termos, ícones e fluxos utilizados são compreensíveis e próximos da realidade do usuário?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
Os elementos apresentados utilizam linguagem clara e familiar ao contexto de sensoriamento remoto e análise ambiental, como “Segmentações Recentes”, “Projetos” e “Modelos”. Os cards organizam as informações de forma semelhante a painéis de monitoramento conhecidos pelos usuários.

**Exemplo da aplicação:** utilização de termos compreensíveis e organização visual semelhante a dashboards reais.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A área de upload utiliza metáforas visuais já conhecidas, como arrastar arquivos para envio (“drag and drop”), além de mensagens simples e diretas como “Selecione uma imagem”.

**Exemplo da aplicação:** área de upload com comportamento semelhante a serviços populares de armazenamento em nuvem.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora os modelos estejam organizados visualmente, nomes técnicos como “DeepLabV3+” e “U-Net” podem não ser claros para usuários sem conhecimento em inteligência artificial.

**Boa prática sugerida:**  
Adicionar descrições simplificadas ou tooltips explicando a finalidade e diferença entre os modelos.

**Exemplo da aplicação:** nomes técnicos exibidos sem explicação complementar.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
A apresentação dos resultados utiliza conceitos próximos da realidade do usuário, como porcentagens de alteração, períodos comparativos e indicadores de crescimento ou redução.

**Exemplo da aplicação:** exibição de métricas como “Expansão Urbana” e “Desmatamento” em formato visual intuitivo.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
A organização cronológica das análises segue uma lógica natural e familiar, semelhante a históricos encontrados em plataformas de arquivos e sistemas de monitoramento.

**Exemplo da aplicação:** cards exibindo data, imagem e modelo utilizado.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
As informações institucionais e descrições de funcionalidades utilizam linguagem clara, explicando o propósito do sistema de forma acessível.

**Exemplo da aplicação:** seções organizadas em tópicos como “Propósito” e “Tecnologias”.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 3 — Controle e Liberdade do Usuário

> **Definição:** Os usuários devem ter liberdade para desfazer ações, cancelar operações e navegar sem dificuldades.
>
> **Verificação:** O sistema oferece formas claras de retornar, cancelar ou corrigir ações?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
O menu lateral permite navegação rápida entre seções, oferecendo liberdade para alternar entre funcionalidades sem perder contexto.

**Exemplo da aplicação:** menu lateral fixo acessível durante toda a navegação.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O usuário pode selecionar novos arquivos facilmente, porém não há botão explícito para cancelar uploads em andamento.

**Boa prática sugerida:**  
Adicionar opção de cancelar envio e remover arquivo selecionado antes do processamento.

**Exemplo da aplicação:** ausência de botão de cancelamento durante upload.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os modelos podem ser alterados livremente antes do processamento, permitindo que o usuário revise sua escolha.

**Exemplo da aplicação:** troca de seleção entre modelos sem restrições.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Os resultados são apresentados corretamente, porém não há ação clara para desfazer comparações ou retornar rapidamente para nova análise.

**Boa prática sugerida:**  
Adicionar botão “Nova Comparação” ou “Voltar” visível na interface.

**Exemplo da aplicação:** ausência de atalhos diretos após visualização dos resultados.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
O usuário pode acessar análises anteriores e navegar livremente entre registros.

**Exemplo da aplicação:** histórico navegável com múltiplos projetos disponíveis.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A navegação pode ser interrompida ou alterada facilmente pelo menu lateral.

**Exemplo da aplicação:** possibilidade de sair da página a qualquer momento.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 4 — Consistência e Padronização

> **Definição:** Os usuários não devem precisar adivinhar se diferentes palavras, situações ou ações significam a mesma coisa.
>
> **Verificação:** O sistema mantém padrões visuais e funcionais consistentes?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
O layout segue o mesmo padrão visual encontrado nas demais telas, utilizando a mesma paleta de cores, menus laterais e estrutura de cards.

**Exemplo da aplicação:** consistência entre menu lateral, títulos e componentes visuais.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
Os botões, campos e áreas interativas seguem o mesmo estilo visual adotado em todo o sistema.

**Exemplo da aplicação:** utilização consistente das cores verdes, bordas arredondadas e tipografia padronizada.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os cards de modelos utilizam o mesmo padrão visual aplicado nos demais elementos do sistema, facilitando reconhecimento e aprendizado da interface.

**Exemplo da aplicação:** bordas, espaçamentos e botões padronizados entre os cards.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os gráficos, indicadores e cards seguem a mesma identidade visual da plataforma, mantendo coerência entre as telas.

**Exemplo da aplicação:** uso consistente de cores, ícones e estilos tipográficos.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
Os registros históricos mantêm a mesma organização visual da Home, reforçando a familiaridade da navegação.

**Exemplo da aplicação:** estrutura de cards semelhante à utilizada em segmentações recentes.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página mantém os mesmos padrões de layout, espaçamento e identidade visual presentes nas demais seções do sistema.

**Exemplo da aplicação:** tipografia e menu lateral consistentes com o restante da plataforma.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 5 — Prevenção de Erros

> **Definição:** O sistema deve prevenir problemas antes que eles aconteçam.
>
> **Verificação:** Existem mecanismos para evitar erros do usuário?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A interface apresenta apenas ações relevantes e bem organizadas, reduzindo a chance de cliques incorretos ou navegação confusa.

**Exemplo da aplicação:** menu lateral claro e organizado.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora o sistema possua validação básica para formatos inválidos, ainda não apresenta mensagens preventivas completas sobre tamanho máximo ou restrições antes do envio.

**Boa prática sugerida:**  
Adicionar validação visual para tipos de arquivos aceitos e limites de upload.

**Exemplo da aplicação:** ausência de alertas preventivos antes do envio.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />
<img width="1419" height="726" alt="image" src="https://github.com/user-attachments/assets/beb3ad3e-37fd-414c-87b4-f87c4a667c38" />


---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
A seleção visual ativa evita dúvidas sobre qual modelo será utilizado no processamento.

**Exemplo da aplicação:** destaque verde no modelo selecionado.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
O sistema não apresenta confirmação antes de iniciar processamentos potencialmente demorados.

**Boa prática sugerida:**  
Adicionar confirmação ou aviso antes de iniciar comparações.

**Exemplo da aplicação:** ausência de confirmação antes do processamento.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
As informações históricas são exibidas de forma organizada, minimizando interpretações incorretas.

**Exemplo da aplicação:** dados organizados em cards padronizados.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A tela possui caráter informativo e não apresenta ações críticas que possam gerar erros.

**Exemplo da aplicação:** página apenas para consulta de informações.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 6 — Reconhecimento em vez de Memorização

> **Definição:** O sistema deve minimizar a necessidade de memorização, deixando opções e informações visíveis.
>
> **Verificação:** Os usuários conseguem reconhecer ações e informações facilmente?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
As principais funcionalidades ficam visíveis no menu lateral e os projetos recentes permanecem acessíveis em cards.

**Exemplo da aplicação:** menu lateral sempre visível.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
Os elementos de upload possuem ícones e instruções claras, reduzindo necessidade de memorização.

**Exemplo da aplicação:** área visual de arrastar e soltar arquivos.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora os modelos estejam visíveis, usuários iniciantes podem não reconhecer facilmente suas diferenças.

**Boa prática sugerida:**  
Adicionar descrições resumidas abaixo de cada modelo.

**Exemplo da aplicação:** modelos apresentados apenas pelo nome técnico.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os indicadores visuais e métricas tornam os resultados fáceis de interpretar sem exigir que o usuário memorize valores anteriores. Os gráficos, legendas e resumos textuais reforçam a compreensão imediata das informações apresentadas.

**Exemplo da aplicação:** percentuais e indicadores coloridos de alteração.

<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
As análises anteriores ficam disponíveis visualmente, evitando que o usuário precise memorizar dados passados.

**Exemplo da aplicação:** histórico completo com miniaturas e datas.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
As informações estão organizadas em blocos visíveis e bem separados.

**Exemplo da aplicação:** divisão clara por tópicos.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 7 — Flexibilidade e Eficiência de Uso

> **Definição:** O sistema deve permitir eficiência tanto para usuários iniciantes quanto experientes.
>
> **Verificação:** O sistema oferece formas rápidas e flexíveis de interação?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
O acesso rápido às funcionalidades principais melhora a eficiência da navegação.

**Exemplo da aplicação:** atalhos visuais no menu lateral.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
O suporte ao arrastar e soltar arquivos acelera o processo de envio.

**Exemplo da aplicação:** upload por drag and drop.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
A troca rápida entre modelos facilita testes e comparações.

**Exemplo da aplicação:** seleção instantânea entre modelos disponíveis.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os resultados são organizados visualmente para rápida interpretação. A exportação rápida em PDF, PNG e CSV aumenta a eficiência para usuários avançados que desejam reutilizar os resultados das análises.

**Exemplo da aplicação:** métricas resumidas em cards.

<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1473" height="862" alt="image" src="https://github.com/user-attachments/assets/4bc54c44-f7db-489b-aa98-90b9a1025b3b" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
O histórico é organizado, porém não possui filtros ou pesquisa para localizar análises rapidamente.

**Boa prática sugerida:**  
Adicionar busca e filtros por data ou modelo.

**Exemplo da aplicação:** ausência de campo de pesquisa.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A estrutura da página facilita leitura rápida das informações.

**Exemplo da aplicação:** organização em blocos objetivos.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 8 — Estética e Design Minimalista

> **Definição:** Interfaces não devem conter informações irrelevantes ou excessivas.
>
> **Verificação:** O design apresenta apenas elementos necessários?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A tela apresenta apenas informações essenciais, sem excesso visual.

**Exemplo da aplicação:** organização limpa dos cards e menu.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A interface de upload é objetiva e direciona o usuário claramente para a ação principal.

**Exemplo da aplicação:** foco visual na área de envio.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os modelos são exibidos de forma organizada e sem excesso de informações técnicas.

**Exemplo da aplicação:** cards limpos e bem distribuídos.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora exista grande quantidade de métricas e gráficos, os insights são organizados em cards e seções bem definidas, mantendo hierarquia visual clara e facilitando a leitura das informações.

**Boa prática sugerida:**  
Organizar métricas em seções recolhíveis ou tabs para reduzir sobrecarga visual em análises mais extensas.

**Exemplo da aplicação:** múltiplos cards e gráficos simultâneos.

<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1473" height="862" alt="image" src="https://github.com/user-attachments/assets/4bc54c44-f7db-489b-aa98-90b9a1025b3b" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
Os registros são apresentados de forma limpa e organizada.

**Exemplo da aplicação:** grid simples e objetivo.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
As informações estão divididas em blocos claros, evitando excesso textual contínuo.

**Exemplo da aplicação:** separação visual por seções.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 9 — Ajudar Usuários a Reconhecer, Diagnosticar e Recuperar-se de Erros

> **Definição:** As mensagens de erro devem ser claras e indicar soluções.
>
> **Verificação:** O sistema auxilia o usuário na recuperação de erros?

---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
A tela inicial possui navegação simples e organizada, porém não apresenta mensagens orientativas caso ocorra falha ao carregar projetos ou análises recentes.

**Boa prática sugerida:**  
Adicionar mensagens de erro amigáveis e ações de recuperação, como “Tentar novamente”.

**Exemplo da aplicação:** ausência de feedback de erro na listagem inicial.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---


## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O sistema exibe alerta ao usuário quando um arquivo inválido é enviado, indicando os formatos aceitos (JPG, PNG ou TIF). Entretanto, a mensagem aparece em um alerta genérico do navegador, sem detalhamento visual integrado à interface.

**Boa prática sugerida:**  
Substituir alertas nativos por mensagens estilizadas dentro da aplicação, indicando claramente o erro e possíveis soluções.

**Exemplo da aplicação:** mensagem de erro ao enviar arquivo em formato inválido.

<img width="1409" height="717" alt="image" src="https://github.com/user-attachments/assets/7377105d-08f9-492c-97d2-7895c234369d" />
<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora a seleção visual dos modelos seja clara, não há mensagens explicativas caso o usuário tente avançar sem selecionar um modelo válido.

**Boa prática sugerida:**  
Adicionar mensagens orientativas como “Selecione um modelo antes de continuar”.

**Exemplo da aplicação:** ausência de feedback de erro relacionado à escolha do modelo.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Não há mensagens orientando o usuário caso ocorra falha no processamento.

**Boa prática sugerida:**  
Exibir mensagens de erro com sugestões de nova tentativa.

**Exemplo da aplicação:** ausência de tratamento visual de erros.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
O histórico apresenta as análises anteriores corretamente, porém não há mensagens de recuperação caso ocorra falha no carregamento dos registros.

**Boa prática sugerida:**  
Adicionar feedback visual para histórico vazio ou erro de carregamento.

**Exemplo da aplicação:** ausência de mensagens de recuperação no histórico.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A tela possui apenas conteúdo informativo, reduzindo significativamente a ocorrência de erros de interação.

**Exemplo da aplicação:** página informativa sem ações críticas.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 10 — Ajuda e Documentação

> **Definição:** O sistema deve oferecer ajuda acessível e documentação quando necessário.
>
> **Verificação:** Existem informações de suporte e orientação disponíveis?

---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
A interface inicial é intuitiva, porém não apresenta tutorial, onboarding ou explicações rápidas sobre as funcionalidades disponíveis.

**Boa prática sugerida:**  
Adicionar guia introdutório ou seção “Primeiros Passos”.

**Exemplo da aplicação:** ausência de ajuda contextual na tela inicial.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A área de upload informa os formatos suportados e orienta claramente o usuário sobre como enviar arquivos.

**Exemplo da aplicação:** instruções visíveis para envio de imagens JPG, PNG e TIF.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os modelos são apresentados visualmente, mas sem documentação explicando suas diferenças ou aplicações ideais.

**Boa prática sugerida:**  
Adicionar descrições resumidas ou botão de ajuda para cada modelo.

**Exemplo da aplicação:** ausência de explicações técnicas simplificadas.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Os resultados são apresentados visualmente, mas faltam orientações explicando o significado detalhado das métricas e gráficos. Ainda assim, os resumos automáticos das mudanças funcionam como ajuda contextual, auxiliando o usuário na interpretação dos resultados apresentados.

**Boa prática sugerida:**  
Adicionar tooltips ou seção explicativa sobre indicadores e métricas.

**Exemplo da aplicação:** ausência de ajuda contextual nos gráficos e resultados.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
O histórico é simples de navegar, porém não possui explicações sobre filtros, organização ou recuperação de análises antigas.

**Boa prática sugerida:**  
Adicionar orientações rápidas ou ajuda contextual sobre uso do histórico.

**Exemplo da aplicação:** ausência de documentação auxiliar na tela de histórico.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página apresenta informações sobre propósito, tecnologias e funcionalidades do sistema, funcionando como documentação básica da plataforma.

**Exemplo da aplicação:** descrição organizada das funcionalidades e objetivos do sistema.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---
