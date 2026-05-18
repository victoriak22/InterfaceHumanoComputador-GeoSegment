# Plano de Execução da Atividade — GeoSegment AI

**Disciplina:** CC8122  
**Prof. Dr.:** Plinio T. Aquino Junior  

---

## 1. Preparação da Avaliação

### Objetivos do Teste

Avaliar a usabilidade do protótipo de alta fidelidade do GeoSegment AI no Figma, verificando:

- Facilidade de aprendizado na primeira interação, sem treinamento prévio
- Eficiência na execução de tarefas por usuários sem experiência no sistema
- Erros e hesitações cometidos durante a navegação
- Satisfação geral com a interface

### Questões Específicas

- Quantos usuários conseguem concluir as tarefas sem ajuda direta?
- O usuário compreende termos técnicos como "MIoU" e "segmentação" sem explicação prévia?
- O usuário se orienta pela barra lateral ou pelos elementos centrais da interface?
- Qual o tempo médio para concluir todas as tarefas? *(sessão durou aproximadamente 3 minutos)*
- Quais são os erros ou hesitações mais comuns durante o uso?

### Escopo

**Telas avaliadas:** Home, Upload de Imagem, Seleção de Modelo, Comparação Temporal e Histórico.

**Tarefas representativas:** upload de imagem, seleção de modelo por precisão, interpretação de resultados, uso da comparação temporal e recuperação de análise anterior pelo histórico.

### Método de Avaliação

Teste de usabilidade por **observação direta remota** (via call com compartilhamento de tela), com aplicação da técnica **Think-Aloud**. Complementado por **avaliação heurística prévia** realizada individualmente pelos 5 integrantes da equipe, com base nas 10 heurísticas de Nielsen.

### Perfil e Número de Participantes

| Participante | Perfil | Método |
|---|---|---|
| Heitor Mendes Bernardes, 21 anos | Usuário leigo, graduando em Marketing, familiarizado com interfaces digitais e redes sociais, sem experiência em análise ambiental e sem treinamento no sistema | Teste de usabilidade com observação remota |
| Deise Araujo | Integrante da equipe, conhecimento em heurísticas de Nielsen | Avaliação heurística |
| Gustavo Dias Vicentin | Integrante da equipe, conhecimento em heurísticas de Nielsen | Avaliação heurística |
| Lucas Rebolças | Integrante da equipe, avaliador do teste com usuário | Avaliação heurística |
| Victor Iak | Integrante da equipe, conhecimento em heurísticas de Nielsen | Avaliação heurística |
| Vinicius Saide | Integrante da equipe, conhecimento em heurísticas de Nielsen | Avaliação heurística |

### Material de Apoio Utilizado

- Protótipo de alta fidelidade no Figma (modo de apresentação, link compartilhado)
- Cinco tarefas descritas em cenário de analista ambiental, apresentadas verbalmente pelo avaliador
- Gravação da sessão via call (compartilhamento de tela do participante)
- Formulários de avaliação heurística individual (10 heurísticas de Nielsen por avaliador)
- Planilha de avaliação de usabilidade com 27 itens (Cores, Conteúdo, Imagens, Instruções, Navegação, Usabilidade)
- Termo de Consentimento Livre e Esclarecido (TCLE), utilizado para garantir consentimento voluntário, privacidade dos dados e autorização para realização das gravações durante o teste;
- Questionário pós-teste aplicado após a execução das tarefas para coleta de percepções, dificuldades, sugestões e nível de satisfação do participante em relação ao GeoSegment AI;

### Ambiente

Sessão remota realizada via call, com o participante compartilhando a tela e o avaliador observando em tempo real. O avaliador (Lucas Rebolças) conduziu a sessão verbalmente, sem demonstrar a execução das tarefas. A avaliação heurística foi realizada individualmente por cada integrante em ambiente próprio, com posterior consolidação em grupo.

---

## 2. Execução do Teste

### Recepção e Contextualização do Participante

O avaliador recebeu o participante na call e forneceu um breve contexto: Heitor foi situado no papel de analista ambiental que recebeu uma imagem da APA Petrópolis e deveria utilizá-la no sistema GeoSegment AI. Não foi realizado treinamento prévio na interface nem demonstração de funcionalidades. Além disso, o participante foi informado sobre os termos de consentimento da pesquisa, autorizando sua participação e o registro das informações necessárias para a condução do teste de usabilidade.### Tarefas Apresentadas ao Participante

| # | Tarefa Apresentada |
|---|---|
| T1 | Acessar o sistema e enviar a imagem para processamento |
| T2 | Antes de processar, escolher o modelo mais preciso disponível e anotar seu valor de MIoU |
| T3 | Com o processamento concluído, descobrir qual classe de uso do solo ocupa a maior área |
| T4 | Verificar se a área urbana cresceu entre este ano e o ano passado usando a comparação temporal |
| T5 | Reacessar uma segmentação realizada há duas semanas pelo histórico |

### Observações Durante a Execução

O avaliador manteve postura neutra durante toda a navegação. A única intervenção ocorreu na **Tarefa 2**, quando o participante solicitou esclarecimento sobre o termo "MIoU" — o avaliador explicou que se tratava da precisão do modelo, sem demonstrar onde encontrar a informação. As demais tarefas foram concluídas de forma espontânea. A sessão foi gravada via compartilhamento de tela.

### Encerramento da Sessão

Ao término das cinco tarefas, o avaliador conduziu uma breve conversa de encerramento, coletando impressões gerais do participante sobre a interface do GeoSegment AI, incluindo aspectos relacionados às cores, fontes, menu lateral, organização visual e facilidade de navegação.

Durante essa etapa, também foram discutidas:

- dificuldades encontradas durante o uso;
- clareza das informações apresentadas;
- compreensão dos modelos de IA;
- percepção geral da experiência de uso da plataforma.

Após o encerramento da sessão de observação, foi enviado ao participante um questionário pós-teste com perguntas relacionadas à satisfação, facilidade de uso, dificuldades percebidas, sugestões de melhoria e avaliação geral do sistema, permitindo complementar os dados qualitativos obtidos durante a observação direta.

---

## 3. Pós-Teste

### Percepções Qualitativas Coletadas na Entrevista de Encerramento

O participante relatou espontaneamente os seguintes pontos:

- A interface é **visualmente agradável**, com cores e fontes adequadas e boa legibilidade
- O **menu lateral foi o principal guia de navegação** em todas as tarefas — o participante ignorou elementos centrais (como o botão "Nova Segmentação" e os insights detalhados) e preferiu os itens da barra lateral, mais diretamente nomeados
- O termo **"MIoU" foi completamente desconhecido**; sugeriu utilizar apenas a palavra "precisão"
- Na Comparação Temporal, considerou que os **valores de mudança detectada deveriam aparecer antes do mapa**, facilitando a leitura imediata dos dados relevantes
- Avaliou a interface como **"didática" e bem escrita**, o que facilita a localização das informações

> Não foi aplicado questionário SUS formal nesta sessão.

---

## 4. Análise dos Dados

### Dados Quantitativos

| Tarefa | Concluída? | Observação |
|---|---|---|
| T1 — Upload de imagem | Sim | Navegou pelo menu lateral ("Upload de Imagem") em vez do botão "Nova Segmentação" |
| T2 — Seleção do modelo mais preciso | Sim *(com intervenção)* | Necessitou de esclarecimento sobre o termo "MIoU" |
| T3 — Classe com maior área | Sim | Identificou nas estatísticas de uso do solo que "floresta" era a maior classe |
| T4 — Comparação temporal | Sim | Utilizou o menu lateral em vez dos insights já disponíveis na tela de resultados |
| T5 — Histórico | Sim | Navegou diretamente ao Histórico e compreendeu a organização por datas |

**Taxa de conclusão:** 5/5 tarefas (100%)  
**Tempo total da sessão:** aproximadamente 3 minutos  
**Intervenções necessárias:** 1 (esclarecimento do termo MIoU)

### Dados Qualitativos — Avaliação Heurística Consolidada (5 avaliadores)

Problemas mais recorrentes, identificados por 3 ou mais avaliadores:

| Problema Identificado | Heurística | Severidade Consenso |
|---|---|:---:|
| Ausência de barra de progresso no upload e no processamento | H1 — Visibilidade do status | 2 — Simples |
| Nomes técnicos "U-Net" e "DeepLabV3+" sem explicação acessível | H2 — Linguagem do usuário | 3 — Grave |
| Sem botão para cancelar upload ou reiniciar comparação | H3 — Controle do usuário | 1 — Cosmético |
| Histórico sem filtros ou campo de busca | H7 — Flexibilidade e eficiência | 2 — Simples |
| Mensagens de erro genéricas do navegador, sem integração visual | H9 — Recuperação de erros | 2 — Simples |
| Sem tutorial, onboarding ou ajuda contextual | H10 — Ajuda e documentação | 2 — Simples |
| Ausência de indicador de progresso em fluxos multi-etapa | Item 4.3 — Instruções | -1 — Não atende |
| Área de login sem suporte a e-mail como ID alternativo | Item 6.7 — Usabilidade | -1 — Não atende |

**Escala de severidade:** 0 = sem importância · 1 = cosmético · 2 = simples · 3 = grave · 4 = catastrófico

---

## 5. Consolidação dos Resultados

### Problemas Mais Frequentes e Críticos

**Terminologia técnica na seleção de modelos**  
O problema de maior recorrência e impacto — confirmado diretamente no teste com usuário — foi o uso do termo "MIoU" sem explicação. O participante não reconheceu o termo, o que exigiu intervenção do avaliador. A substituição por "precisão" foi validada pelo próprio usuário durante a sessão.

**Prevalência do menu lateral como guia primário de navegação**  
O participante ignorou elementos de destaque na área central (botão "Nova Segmentação", insights de comparação disponíveis na tela de resultados) e preferiu consistentemente os rótulos diretos da barra lateral. Isso sugere que o fluxo principal precisa de reforço visual ou que os rótulos centrais devem ser revisados para maior clareza.

### Recomendações de Melhoria por Prioridade

**Alta prioridade** *(problema grave confirmado por avaliadores e no teste com usuário)*

- Substituir ou complementar nomes técnicos dos modelos com descrições funcionais em linguagem acessível, indicando claramente qual possui "maior precisão"
- Adicionar barra de progresso visível durante upload e processamento de imagens

**Média prioridade** *(identificado por múltiplos avaliadores)*

- Adicionar campo de busca e filtros por data, nome ou modelo no Histórico
- Integrar mensagens de erro à interface, substituindo alertas nativos do navegador por feedback visual contextualizado
- Incluir botão "Nova Análise" ou "Voltar" claramente visível após a visualização dos resultados na Comparação Temporal
- Adicionar onboarding ou ajuda contextual mínima para novos usuários (ex.: seção "Primeiros Passos")
- Incluir indicadores de progresso em fluxos que envolvam múltiplas etapas

**Baixa prioridade** *(aspectos cosméticos ou de refinamento)*

- Adicionar indicador de seção ativa ou âncoras na tela Sobre durante a rolagem
- Padronizar espaçamentos e tamanhos de componentes entre cards de diferentes telas
