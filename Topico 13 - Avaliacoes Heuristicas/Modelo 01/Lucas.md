# Heurística 1 — Visibilidade do Status do Sistema

> **Definição:** O sistema deve sempre manter os usuários informados sobre o que está acontecendo, através de feedback apropriado em um tempo razoável.
>
> **Verificação:** Os usuários são mantidos informados sobre o progresso do sistema com apropriado feedback em um tempo razoável?
---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
A página inicial apresenta informações relevantes sobre análises recentes, porém não existe atualização automática ou indicação temporal de última sincronização dos dados exibidos.

**Boa prática sugerida:**  
Adicionar informação de “última atualização” ou atualização dinâmica dos cards.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A tela apresenta claramente o estado inicial do sistema e mantém a área de upload destacada visualmente. A disposição dos elementos permite ao usuário compreender rapidamente a ação esperada.

**Exemplo da aplicação:** área centralizada de upload com indicação textual do estado atual.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
O sistema fornece feedback imediato quando um modelo é selecionado, utilizando mudança de borda, contraste e atualização textual no botão principal.

**Exemplo da aplicação:** alteração visual instantânea após selecionar um modelo de segmentação.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Apesar dos resultados finais serem apresentados de forma clara, durante o processamento das comparações não há indicação do tempo restante ou do estágio atual da análise.

**Boa prática sugerida:**  
Exibir etapas do processamento, como “Comparando imagens”, “Gerando métricas” e “Finalizando análise”.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
Os registros anteriores apresentam miniaturas, datas e identificação dos modelos utilizados, oferecendo clareza sobre as análises realizadas anteriormente.

**Exemplo da aplicação:** cards organizados contendo resumo visual das análises salvas.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora a página possua conteúdo organizado, a navegação longa pode dificultar a percepção do posicionamento do usuário dentro da tela.

**Boa prática sugerida:**  
Adicionar menu interno fixo ou indicador de seção ativa durante a rolagem.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 2: Correspondência entre o Sistema e o Mundo Real

> **Definição:** O sistema deve falar a linguagem do usuário, utilizando palavras, conceitos e convenções familiares, seguindo a lógica do mundo real.
>
> **Verificação:** Os termos, ícones e fluxos utilizados são compreensíveis e próximos da realidade do usuário?

---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora a organização visual seja familiar, alguns termos utilizados podem não ser imediatamente compreendidos por usuários sem experiência em análise geoespacial.

**Boa prática sugerida:**  
Adicionar explicações rápidas ou glossário para termos mais específicos.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A interação de upload segue convenções conhecidas em aplicações web modernas, facilitando a adaptação do usuário ao sistema.

**Exemplo da aplicação:** área de drag and drop centralizada e intuitiva.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os nomes dos modelos são excessivamente técnicos e não explicam de forma prática qual resultado cada modelo entrega.

**Boa prática sugerida:**  
Apresentar exemplos de uso ou breve descrição funcional abaixo de cada modelo.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os gráficos e indicadores seguem padrões próximos de relatórios ambientais profissionais, tornando os resultados compreensíveis visualmente.

**Exemplo da aplicação:** utilização de indicadores percentuais e comparação temporal entre períodos.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />


---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora o histórico siga uma lógica cronológica familiar, a ausência de categorias ou filtros pode dificultar o entendimento em grandes volumes de análises.

**Boa prática sugerida:**  
Adicionar agrupamentos por data, projeto ou modelo utilizado.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Parcialmente Atendida

**Justificativa:**  
Algumas descrições utilizam termos técnicos relacionados a inteligência artificial e sensoriamento remoto sem contextualização simplificada.

**Boa prática sugerida:**  
Adicionar explicações mais acessíveis para usuários sem conhecimento técnico.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 3: Controle e Liberdade do Usuário

> **Definição:** Os usuários devem ter liberdade para desfazer ações, cancelar operações e navegar sem dificuldades.
>
> **Verificação:** O sistema oferece formas claras de retornar, cancelar ou corrigir ações?
---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora a navegação seja simples, não há atalhos rápidos para retornar diretamente às últimas análises realizadas.

**Boa prática sugerida:**  
Adicionar acesso rápido às atividades recentes diretamente na dashboard.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O sistema não oferece mecanismo de desfazer após seleção incorreta da imagem ou interrupção clara do processamento.

**Boa prática sugerida:**  
Adicionar botão para remover imagem selecionada antes do envio final.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
A alteração entre modelos ocorre de forma livre e sem necessidade de reiniciar o processo de seleção.

**Exemplo da aplicação:** seleção dinâmica entre diferentes modelos disponíveis.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Não existem controles claros para retornar aos parâmetros anteriores utilizados na comparação.

**Boa prática sugerida:**  
Adicionar histórico de comparações recentes ou botão “Voltar para configuração”.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
Apesar da navegação livre entre registros, não existem ações rápidas para excluir, restaurar ou reorganizar análises.

**Boa prática sugerida:**  
Adicionar ações contextuais nos cards do histórico.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
O usuário pode interromper a leitura e navegar para outras páginas sem restrições.

**Exemplo da aplicação:** navegação lateral persistente.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 4 — Consistência e Padronização

> **Definição:** Os usuários não devem precisar adivinhar se diferentes palavras, situações ou ações significam a mesma coisa.
>
> **Verificação:** O sistema mantém padrões visuais e funcionais consistentes?
---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora exista consistência visual geral, alguns cards apresentam diferenças sutis de alinhamento e quantidade de informações.

**Boa prática sugerida:**  
Padronizar espaçamentos e quantidade de conteúdo exibido nos cards.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A tela segue o mesmo padrão visual e funcional das demais páginas, mantendo identidade consistente.

**Exemplo da aplicação:** repetição de estilos visuais utilizados em toda plataforma.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os nomes técnicos dos modelos destoam da linguagem mais simples presente em outras partes do sistema.

**Boa prática sugerida:**  
Adicionar descrições mais amigáveis para equilibrar a comunicação visual e textual.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
A quantidade elevada de gráficos e indicadores simultâneos pode gerar sensação de excesso visual em comparação às demais telas.

**Boa prática sugerida:**  
Simplificar agrupamentos visuais ou dividir conteúdos em seções menores.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
A estrutura dos cards segue padrão semelhante ao utilizado na Home, mantendo coerência visual.

**Exemplo da aplicação:** repetição de miniaturas, badges e estilo de navegação.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Parcialmente Atendida

**Justificativa:**  
Algumas seções possuem espaçamentos diferentes do restante da plataforma, causando pequena quebra de padronização.

**Boa prática sugerida:**  
Uniformizar margens e alinhamentos entre blocos de conteúdo.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 5: Prevenção de Erros

> **Definição:** O sistema deve prevenir problemas antes que eles aconteçam.
>
> **Verificação:** Existem mecanismos para evitar erros do usuário?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A interface evita excesso de opções na tela inicial, facilitando entendimento e diminuindo ações incorretas.

**Exemplo da aplicação:** organização limpa e objetiva da dashboard.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O usuário consegue enviar arquivos facilmente, porém faltam mensagens preventivas antes do upload para evitar erros comuns.

**Boa prática sugerida:**  
Exibir mensagens como “Apenas arquivos JPG e PNG são permitidos”.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os modelos possuem nomes técnicos que podem levar usuários iniciantes a escolher opções inadequadas sem entender diferenças.

**Boa prática sugerida:**  
Adicionar explicações simples sobre cada modelo antes do processamento.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Não existe aviso sobre tempo estimado da análise, o que pode fazer o usuário pensar que ocorreu falha no sistema.

**Boa prática sugerida:**  
Adicionar mensagem informando duração aproximada do processamento.

<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
Os registros históricos são organizados de maneira clara, reduzindo confusão durante acesso às análises.

**Exemplo da aplicação:** separação visual entre projetos e datas.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
Como não existem ações críticas nesta tela, o risco de erro do usuário é baixo.

**Exemplo da aplicação:** página apenas para leitura de informações.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 6: Reconhecimento em vez de Memorização

> **Definição:** O sistema deve minimizar a necessidade de memorização, deixando opções e informações visíveis.
>
> **Verificação:** Os usuários conseguem reconhecer ações e informações facilmente?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
Os projetos recentes permanecem visíveis na tela inicial, facilitando o acesso rápido sem necessidade de lembrar informações anteriores.

**Exemplo da aplicação:** cards com dados recentes exibidos logo na Home.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
Os botões e ícones utilizados seguem padrões conhecidos de outras plataformas, tornando o reconhecimento intuitivo.

**Exemplo da aplicação:** uso de ícones de upload e área de arrastar arquivos.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Usuários iniciantes podem ter dificuldade em reconhecer rapidamente as diferenças entre os modelos disponíveis.

**Boa prática sugerida:**  
Adicionar exemplos simples mostrando quando utilizar cada modelo.

**Exemplo da aplicação:** ausência de explicações visuais complementares.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os gráficos e legendas permitem compreender os resultados sem necessidade de memorizar números ou dados anteriores.

**Exemplo da aplicação:** gráficos comparativos e indicadores visuais claros.

<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
As análises anteriores ficam registradas visualmente, permitindo reconhecer projetos facilmente.

**Exemplo da aplicação:** miniaturas e datas exibidas nos cards.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora o conteúdo esteja separado em tópicos, algumas informações técnicas podem dificultar reconhecimento imediato para usuários leigos.

**Boa prática sugerida:**  
Simplificar parte das descrições técnicas.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 7: Flexibilidade e Eficiência de Uso

> **Definição:** O sistema deve permitir eficiência tanto para usuários iniciantes quanto experientes.
>
> **Verificação:** O sistema oferece formas rápidas e flexíveis de interação?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A organização simples da página inicial permite acesso rápido às principais funções sem exigir muitos cliques.

**Exemplo da aplicação:** menu lateral sempre disponível.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
O envio de arquivos ocorre de maneira rápida através do arrastar e soltar imagens diretamente na área indicada.

**Exemplo da aplicação:** upload simplificado por drag and drop.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Usuários iniciantes podem demorar para escolher um modelo por falta de explicações rápidas sobre cada opção.

**Boa prática sugerida:**  
Adicionar pequenas descrições explicando quando usar cada modelo.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os resultados resumidos em gráficos e cards permitem interpretação rápida sem necessidade de análise detalhada.

**Exemplo da aplicação:** métricas organizadas visualmente.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
Não existem filtros ou pesquisa rápida para encontrar análises antigas de forma eficiente.

**Boa prática sugerida:**  
Adicionar campo de busca e ordenação por data.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página permite leitura rápida por apresentar conteúdo dividido em partes menores e organizadas.

**Exemplo da aplicação:** textos separados em blocos objetivos.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 8: Estética e Design Minimalista

> **Definição:** Interfaces não devem conter informações irrelevantes ou excessivas.
>
> **Verificação:** O design apresenta apenas elementos necessários?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A organização dos elementos facilita entendimento rápido sem excesso visual.

**Exemplo da aplicação:** cards organizados e menu lateral discreto.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A tela possui foco claro na ação principal, evitando elementos desnecessários.

**Exemplo da aplicação:** área centralizada para envio de arquivos.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora organizada, a tela poderia apresentar descrições menores para evitar excesso de texto técnico.

**Boa prática sugerida:**  
Utilizar textos mais curtos e objetivos nos cards.

**Exemplo da aplicação:** presença de nomes técnicos nos modelos.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
A quantidade de indicadores e gráficos pode dificultar leitura rápida das informações mais importantes.

**Boa prática sugerida:**  
Priorizar apenas métricas principais na visualização inicial.

**Exemplo da aplicação:** diversos gráficos exibidos ao mesmo tempo.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
A tela apresenta apenas informações necessárias para identificação das análises.

**Exemplo da aplicação:** miniaturas e títulos organizados em cards simples.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A divisão em tópicos reduz excesso textual contínuo e melhora leitura.

**Exemplo da aplicação:** separação clara entre seções informativas.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 9: Ajudar Usuários a Reconhecer, Diagnosticar e Recuperar-se de Erros

> **Definição:** As mensagens de erro devem ser claras e indicar soluções.
>
> **Verificação:** O sistema auxilia o usuário na recuperação de erros?

---

## Tela: Home

**Status:** Não Atendida

**Justificativa:**  
A tela inicial não mostra mensagens explicativas caso os dados não carreguem corretamente.

**Boa prática sugerida:**  
Adicionar feedback visual indicando falha de conexão ou carregamento.

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
O sistema informa ao usuário quando o arquivo enviado não é compatível, ajudando na identificação do problema.

**Exemplo da aplicação:** alerta indicando formatos aceitos.

<img width="1409" height="717" alt="image" src="https://github.com/user-attachments/assets/7377105d-08f9-492c-97d2-7895c234369d" />

---

## Tela: Seleção de Modelo

**Status:** Não Atendida

**Justificativa:**  
Faltam mensagens explicativas orientando o usuário caso nenhum modelo seja escolhido antes de continuar.

**Boa prática sugerida:**  
Exibir mensagem simples próxima ao botão de avanço.

---

## Tela: Comparação Temporal

**Status:** Não Atendida

**Justificativa:**  
O usuário não recebe orientações claras caso ocorra falha no processamento ou demora excessiva.

**Boa prática sugerida:**  
Adicionar mensagens indicando o que aconteceu e como resolver.

---

## Tela: Histórico

**Status:** Não Atendida

**Justificativa:**  
Não há mensagens informando quando o histórico está vazio ou indisponível.

**Boa prática sugerida:**  
Adicionar aviso como “Nenhuma análise encontrada”.

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página é apenas informativa e praticamente não apresenta risco de erros de interação.

**Exemplo da aplicação:** leitura simples de informações.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 10: Ajuda e Documentação

> **Definição:** O sistema deve oferecer ajuda acessível e documentação quando necessário.
>
> **Verificação:** Existem informações de suporte e orientação disponíveis?

---

## Tela: Home

**Status:** Não Atendida

**Justificativa:**  
Embora a interface seja intuitiva, não há orientações iniciais explicando fluxo de uso da plataforma.

**Boa prática sugerida:**  
Adicionar seção “Como começar” para novos usuários.

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
As instruções de envio estão visíveis e ajudam o usuário a entender rapidamente como utilizar a funcionalidade.

**Exemplo da aplicação:** explicação dos formatos permitidos.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Usuários iniciantes podem não compreender as diferenças entre os modelos apresentados.

**Boa prática sugerida:**  
Adicionar exemplos simples mostrando quando utilizar cada modelo.

**Exemplo da aplicação:** ausência de explicações complementares.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Os gráficos são visuais, porém faltam orientações explicando significado de indicadores mais técnicos.

**Boa prática sugerida:**  
Adicionar descrições rápidas próximas dos gráficos.

**Exemplo da aplicação:** ausência de ajuda interpretativa.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
A navegação é simples, mas faltam orientações sobre organização e recuperação de análises anteriores.

**Boa prática sugerida:**  
Adicionar explicações rápidas sobre filtros e histórico.

**Exemplo da aplicação:** ausência de suporte contextual.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página fornece explicações gerais sobre funcionamento e propósito do sistema.

**Exemplo da aplicação:** descrição das funcionalidades e objetivos da plataforma.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />
