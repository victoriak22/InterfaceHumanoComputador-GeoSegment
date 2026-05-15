# Heurística 1 — Visibilidade do Status do Sistema

> **Definição:** O sistema deve sempre manter os usuários informados sobre o que está acontecendo, através de feedback apropriado em um tempo razoável.
>
> **Verificação:** Os usuários são mantidos informados sobre o progresso do sistema com apropriado feedback em um tempo razoável?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A dashboard inicial apresenta informações organizadas em cards, permitindo que o usuário identifique rapidamente os projetos recentes e os modelos utilizados. O destaque visual da navegação lateral facilita a identificação da página atual dentro do sistema.

**Exemplo da aplicação:** menu lateral destacando a seção ativa e cards com informações resumidas das análises.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
A interface informa ao usuário que nenhuma imagem foi enviada através do texto “Aguardando upload”. Entretanto, após selecionar o arquivo, o sistema não apresenta confirmação imediata do andamento do envio ou do processamento da imagem.

**Boa prática sugerida:**  
Adicionar feedback visual contínuo durante o upload, como spinner, barra de progresso ou mensagem dinâmica indicando o processamento do arquivo.

**Exemplo da aplicação:** área de upload com status inicial exibido, porém sem progresso visível durante o carregamento.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os modelos disponíveis possuem diferenciação visual clara quando selecionados. O sistema também atualiza automaticamente o botão principal conforme a escolha realizada, reforçando a percepção de estado atual.

**Exemplo da aplicação:** destaque verde no modelo selecionado e alteração do botão para refletir o modelo ativo.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os resultados das análises são exibidos de maneira objetiva através de métricas, percentuais e indicadores visuais coloridos. O usuário consegue compreender rapidamente quais alterações foram detectadas pelo sistema.

**Exemplo da aplicação:** exibição de percentuais positivos e negativos relacionados às mudanças identificadas entre períodos analisados.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora os registros anteriores sejam apresentados em cards organizados com informações importantes, não existe indicação de carregamento ou atualização caso o histórico demore para ser exibido.

**Boa prática sugerida:**  
Adicionar skeleton loading ou mensagem de carregamento enquanto os registros históricos são recuperados.

**Exemplo da aplicação:** listagem de análises anteriores sem indicador de atualização da página.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A estrutura da página organiza o conteúdo em seções bem definidas, permitindo leitura contínua e entendimento do propósito do sistema. O menu lateral também auxilia na localização da seção atual.

**Exemplo da aplicação:** separação clara entre propósito, funcionalidades e tecnologias utilizadas.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 2: Correspondência entre o Sistema e o Mundo Real

> **Definição:** O sistema deve falar a linguagem do usuário, utilizando palavras, conceitos e convenções familiares, seguindo a lógica do mundo real.
>
> **Verificação:** Os termos, ícones e fluxos utilizados são compreensíveis e próximos da realidade do usuário?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A dashboard utiliza elementos familiares encontrados em plataformas de monitoramento e análise de dados, facilitando a compreensão do usuário. Termos como “Projetos”, “Segmentações” e “Modelos” mantêm coerência com o domínio da aplicação.

**Exemplo da aplicação:** organização em cards semelhantes a sistemas de monitoramento e análise.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A funcionalidade de arrastar e soltar arquivos segue um padrão amplamente utilizado em aplicações web modernas, tornando a interação intuitiva mesmo para usuários iniciantes.

**Exemplo da aplicação:** área de upload semelhante a serviços de armazenamento em nuvem.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os modelos estão organizados de forma clara, porém os nomes técnicos utilizados podem dificultar o entendimento de usuários sem experiência em inteligência artificial.

**Boa prática sugerida:**  
Adicionar descrições simplificadas explicando a principal função de cada modelo.

**Exemplo da aplicação:** utilização de nomes técnicos como “U-Net” e “DeepLabV3+”.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
As informações apresentadas seguem uma lógica próxima de relatórios ambientais e monitoramento territorial reais, utilizando métricas e indicadores compreensíveis.

**Exemplo da aplicação:** indicadores de crescimento, redução e métricas percentuais.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
A organização cronológica das análises segue um padrão comum em plataformas de gerenciamento de arquivos e históricos de atividades.

**Exemplo da aplicação:** cards contendo data, miniatura da imagem e modelo utilizado.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página apresenta informações institucionais utilizando linguagem clara e acessível, permitindo entendimento do propósito da plataforma mesmo para usuários não técnicos.

**Exemplo da aplicação:** divisão do conteúdo em tópicos organizados.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 3: Controle e Liberdade do Usuário

> **Definição:** Os usuários devem ter liberdade para desfazer ações, cancelar operações e navegar sem dificuldades.
>
> **Verificação:** O sistema oferece formas claras de retornar, cancelar ou corrigir ações?
---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A presença do menu lateral fixo facilita a troca rápida entre páginas, permitindo que o usuário navegue livremente sem necessidade de retornar manualmente para a tela inicial.

**Exemplo da aplicação:** navegação contínua entre Home, Histórico e Upload.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O sistema permite substituir facilmente uma imagem enviada, porém não apresenta opção clara para cancelar o envio durante o processo.

**Boa prática sugerida:**  
Adicionar botão “Cancelar Upload” visível durante o envio da imagem.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os modelos podem ser alterados livremente antes da execução, garantindo flexibilidade ao usuário na tomada de decisão.

**Exemplo da aplicação:** troca instantânea entre modelos sem bloqueios.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Após visualizar os resultados, não existe ação rápida para iniciar uma nova comparação ou editar os parâmetros utilizados anteriormente.

**Boa prática sugerida:**  
Adicionar botão “Refazer Comparação” ou “Editar Análise”.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
O usuário pode acessar análises anteriores livremente, retornando entre registros sem restrições.

**Exemplo da aplicação:** histórico navegável com múltiplos cards acessíveis.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A navegação permanece acessível durante toda a leitura, permitindo saída imediata da página sem perda de contexto.

**Exemplo da aplicação:** menu lateral fixo durante navegação.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 4: Consistência e Padronização

> **Definição:** Os usuários não devem precisar adivinhar se diferentes palavras, situações ou ações significam a mesma coisa.
>
> **Verificação:** O sistema mantém padrões visuais e funcionais consistentes?

---

## Tela: Home

**Status:** Atendida

**Justificativa:**  
A tela inicial mantém o mesmo padrão visual presente em todo o sistema, utilizando menu lateral fixo, cards organizados e paleta de cores consistente.

**Exemplo da aplicação:** repetição dos mesmos estilos de títulos, cores e componentes visuais.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
Os botões e áreas interativas seguem o mesmo padrão visual das demais telas, facilitando reconhecimento e aprendizado do usuário.

**Exemplo da aplicação:** uso consistente de cores verdes, bordas arredondadas e tipografia semelhante.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os cards dos modelos seguem a mesma estrutura visual aplicada em outros componentes da plataforma, mantendo consistência entre espaçamentos, botões e destaques.

**Exemplo da aplicação:** padronização visual entre cards e botões de seleção.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os gráficos e indicadores mantêm identidade visual alinhada com o restante do sistema, utilizando mesmas cores, estilos de cards e organização visual.

**Exemplo da aplicação:** consistência entre gráficos, métricas e indicadores visuais.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
A organização dos cards segue o mesmo padrão da Home, reforçando familiaridade e previsibilidade na navegação.

**Exemplo da aplicação:** utilização consistente de miniaturas, badges e espaçamentos.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página mantém alinhamento visual com as demais telas, preservando identidade visual, menu lateral e padronização tipográfica.

**Exemplo da aplicação:** mesma estrutura visual utilizada em toda plataforma.

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
A página inicial possui navegação simples e organizada, reduzindo chances de o usuário clicar em opções erradas.

**Exemplo da aplicação:** menu lateral separado por categorias claras.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O sistema aceita apenas formatos válidos, porém não informa claramente antes do envio os tamanhos de arquivos permitidos.

**Boa prática sugerida:**  
Mostrar mensagem visível com tamanho máximo do arquivo.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />
<img width="1419" height="726" alt="image" src="https://github.com/user-attachments/assets/beb3ad3e-37fd-414c-87b4-f87c4a667c38" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
O modelo escolhido fica destacado visualmente, evitando que o usuário processe a imagem utilizando opção errada.

**Exemplo da aplicação:** destaque em verde no modelo selecionado.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
A análise pode ser iniciada sem confirmação prévia, o que pode gerar processamento desnecessário por engano.

**Boa prática sugerida:**  
Adicionar aviso de confirmação antes de iniciar comparações demoradas.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
As análises ficam organizadas visualmente, reduzindo risco de o usuário abrir arquivos errados.

**Exemplo da aplicação:** cards separados por projeto e data.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página possui apenas informações descritivas, sem ações críticas que possam causar erros.

**Exemplo da aplicação:** conteúdo apenas informativo.

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
As funções principais ficam sempre visíveis no menu lateral, permitindo que o usuário encontre rapidamente o que precisa sem decorar caminhos.

**Exemplo da aplicação:** menu lateral fixo durante toda navegação.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A área de upload utiliza ícones conhecidos e instruções simples, facilitando o entendimento até para usuários iniciantes.

**Exemplo da aplicação:** área visual de arrastar arquivos com instruções claras.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os modelos ficam visíveis na tela, porém os nomes técnicos dificultam o reconhecimento imediato da função de cada um.

**Boa prática sugerida:**  
Adicionar explicações simples abaixo de cada modelo.

**Exemplo da aplicação:** modelos exibidos apenas por nomes técnicos.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os resultados utilizam cores, gráficos e porcentagens que ajudam o usuário a entender rapidamente as mudanças encontradas.

**Exemplo da aplicação:** indicadores coloridos de aumento e redução das áreas.

<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
As análises anteriores ficam disponíveis visualmente, evitando que o usuário precise lembrar datas ou projetos manualmente.

**Exemplo da aplicação:** cards com miniaturas, datas e nomes dos projetos.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
As informações estão organizadas em blocos separados e fáceis de localizar.

**Exemplo da aplicação:** conteúdo dividido em tópicos claros.

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
As principais funções ficam acessíveis rapidamente pelo menu lateral, facilitando navegação sem etapas desnecessárias.

**Exemplo da aplicação:** atalhos rápidos disponíveis na lateral da interface.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
O recurso de arrastar arquivos diretamente para a área de upload agiliza o processo de envio.

**Exemplo da aplicação:** suporte ao drag and drop.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
A troca entre modelos ocorre rapidamente, permitindo testes sem dificuldade.

**Exemplo da aplicação:** alteração instantânea da seleção dos modelos.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Atendida

**Justificativa:**  
Os resultados ficam organizados de forma clara e a exportação em diferentes formatos ajuda usuários avançados a reutilizarem os dados com facilidade.

**Exemplo da aplicação:** exportação em PDF, PNG e CSV.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
Embora organizado, o histórico não possui ferramentas rápidas de busca para localizar análises específicas.

**Boa prática sugerida:**  
Adicionar filtros por data, nome do projeto ou modelo utilizado.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
As informações estão organizadas em blocos objetivos, permitindo leitura rápida e eficiente.

**Exemplo da aplicação:** divisão clara entre tópicos informativos.

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
A tela inicial apresenta apenas informações importantes para o usuário, mantendo visual limpo e organizado.

**Exemplo da aplicação:** menu lateral simples e cards bem distribuídos.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A interface direciona atenção para a principal ação da página, evitando distrações desnecessárias.

**Exemplo da aplicação:** destaque visual na área de upload.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Atendida

**Justificativa:**  
Os modelos estão organizados em cards simples e objetivos, facilitando leitura rápida das opções disponíveis.

**Exemplo da aplicação:** distribuição limpa dos modelos na tela.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Apesar da boa organização visual, a quantidade elevada de gráficos e métricas pode causar excesso de informação para alguns usuários.

**Boa prática sugerida:**  
Separar resultados em abas ou seções recolhíveis.

**Exemplo da aplicação:** múltiplos gráficos exibidos simultaneamente.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Atendida

**Justificativa:**  
Os registros aparecem organizados em uma grade limpa, facilitando leitura e navegação.

**Exemplo da aplicação:** histórico visual sem excesso de informações.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
O conteúdo está dividido em blocos menores, facilitando leitura sem sobrecarregar o usuário.

**Exemplo da aplicação:** organização visual em tópicos separados.

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
Caso ocorram falhas no carregamento de projetos ou análises recentes, o sistema não apresenta mensagens explicando o problema ao usuário.

**Boa prática sugerida:**  
Adicionar mensagens simples como “Não foi possível carregar os dados” com botão “Tentar novamente”.

---

## Tela: Upload de Imagem

**Status:** Parcialmente Atendida

**Justificativa:**  
O sistema informa quando o arquivo possui formato inválido, porém utiliza alerta genérico do navegador, dificultando entendimento mais amigável do erro.

**Boa prática sugerida:**  
Exibir mensagens visuais integradas à interface explicando como corrigir o problema.

**Exemplo da aplicação:** alerta ao enviar arquivo incompatível.

<img width="1409" height="717" alt="image" src="https://github.com/user-attachments/assets/7377105d-08f9-492c-97d2-7895c234369d" />
<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Não Atendida

**Justificativa:**  
O sistema não orienta claramente o usuário caso ele tente continuar sem selecionar um modelo válido.

**Boa prática sugerida:**  
Adicionar aviso como “Escolha um modelo antes de continuar”.

---

## Tela: Comparação Temporal

**Status:** Não Atendida

**Justificativa:**  
Não existem mensagens claras caso aconteça falha durante processamento das análises temporais.

**Boa prática sugerida:**  
Mostrar mensagens de erro com orientação para repetir a operação.

---

## Tela: Histórico

**Status:** Não Atendida

**Justificativa:**  
O sistema não apresenta mensagens informando ao usuário quando ocorre falha no carregamento do histórico.

**Boa prática sugerida:**  
Adicionar mensagens de erro e atualização automática da página.

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
Por ser uma página apenas informativa, existem poucas possibilidades de erro durante utilização.

**Exemplo da aplicação:** ausência de ações críticas na interface.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />

---

# Heurística 10: Ajuda e Documentação

> **Definição:** O sistema deve oferecer ajuda acessível e documentação quando necessário.
>
> **Verificação:** Existem informações de suporte e orientação disponíveis?

---

## Tela: Home

**Status:** Parcialmente Atendida

**Justificativa:**  
A navegação é simples, porém usuários iniciantes podem ter dificuldade para entender rapidamente todas as funcionalidades disponíveis.

**Boa prática sugerida:**  
Adicionar tutorial inicial ou explicações rápidas na primeira utilização.

**Exemplo da aplicação:** ausência de onboarding na página inicial.

<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/5169d6ee-62c5-45c2-9e1d-6779956d0071" />

---

## Tela: Upload de Imagem

**Status:** Atendida

**Justificativa:**  
A tela apresenta instruções claras sobre formatos aceitos e forma correta de envio das imagens.

**Exemplo da aplicação:** orientações visíveis para upload de arquivos JPG, PNG e TIF.

<img width="1433" height="632" alt="image" src="https://github.com/user-attachments/assets/dc8bf6ba-87bc-4534-9e5d-12a064554849" />

---

## Tela: Seleção de Modelo

**Status:** Parcialmente Atendida

**Justificativa:**  
Os modelos são apresentados visualmente, porém faltam explicações simples sobre diferenças e melhores usos.

**Boa prática sugerida:**  
Adicionar botão de ajuda ou pequenas descrições abaixo dos modelos.

**Exemplo da aplicação:** ausência de documentação auxiliar.

<img width="1386" height="751" alt="image" src="https://github.com/user-attachments/assets/1bc90aeb-3c79-465a-84ab-45d00780cf91" />

---

## Tela: Comparação Temporal

**Status:** Parcialmente Atendida

**Justificativa:**  
Os resultados são bem apresentados visualmente, mas não existem explicações detalhadas sobre métricas e gráficos exibidos.

**Boa prática sugerida:**  
Adicionar tooltips ou seção explicando indicadores apresentados.

**Exemplo da aplicação:** ausência de ajuda contextual nos gráficos.

<img width="1387" height="806" alt="image" src="https://github.com/user-attachments/assets/0d38944c-5b1c-4c44-8850-0ad9b1a04708" />
<img width="1423" height="823" alt="image" src="https://github.com/user-attachments/assets/6083fdc3-c0ec-4e5a-8d8a-20b52f1be943" />
<img width="1412" height="855" alt="image" src="https://github.com/user-attachments/assets/a4f525bf-0e5f-44ee-8da6-b838f0b5e48a" />
<img width="1348" height="868" alt="image" src="https://github.com/user-attachments/assets/306f20c0-e479-40a7-8e61-d50c07ca2496" />
<img width="1408" height="867" alt="image" src="https://github.com/user-attachments/assets/24a29cd9-d9a2-44e0-bf53-299bd8e2ed80" />

---

## Tela: Histórico

**Status:** Parcialmente Atendida

**Justificativa:**  
O histórico é simples de usar, porém não existem orientações sobre filtros, pesquisa ou recuperação de análises.

**Boa prática sugerida:**  
Adicionar explicações rápidas sobre funcionamento do histórico.

**Exemplo da aplicação:** ausência de ajuda contextual.

<img width="1473" height="722" alt="image" src="https://github.com/user-attachments/assets/01ed724d-d362-4d52-9d14-78e9165793c0" />

---

## Tela: Sobre

**Status:** Atendida

**Justificativa:**  
A página reúne informações sobre funcionalidades, objetivos e tecnologias da plataforma, funcionando como documentação básica.

**Exemplo da aplicação:** explicação organizada do sistema.

<img width="1300" height="802" alt="image" src="https://github.com/user-attachments/assets/e337c93c-6184-424a-ba70-87ad590d556a" />
