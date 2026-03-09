# Telas no Figma – GeoSegment AI

Link para o projeto de telas do GeoSegment AI no Figma (Figma Make):

**[GeoSegment AI – Web App Screens](https://www.figma.com/make/tk7gEbKUrLuOqVWZkam4q1/GeoSegment-AI-Web-App-Screens?t=sALQZCZuFH2M91k4-1)**

Para editar ou ver todas as telas, abra o link no Figma (conta necessária).

## Sumário

- [Fundamentação do design (princípios e diretrizes de IHC)](#fundamentação-do-design-princípios-e-diretrizes-de-ihc)
- [Padrões de interface utilizados](#padrões-de-interface-utilizados)
- [Imagens das telas (design) e vínculo a personas e cenários](#imagens-das-telas-design-e-vínculo-a-personas-e-cenários)
  - [Home inicial](#home-inicial)
  - [Upload de imagem](#upload-de-imagem)
  - [Seleção de rede](#seleção-de-rede)
  - [Dashboard](#dashboard)

---

## Fundamentação do design (princípios e diretrizes de IHC)

O protótipo aplica princípios de usabilidade (Nielsen; Shneiderman) e decisões alinhadas à análise de concorrência (Tópico 02):

- **Visibilidade do status do sistema:** Indicadores de progresso no upload e no processamento; estados claros (pronto, processando, concluído) para que o usuário saiba em que etapa está.
- **Consistência e padrões:** Navegação previsível (Home → Upload → Seleção de rede → Dashboard); uso consistente de botões, rótulos e hierarquia visual.
- **Prevenção de erros e feedback:** Validação de formato/tamanho de arquivo no upload; mensagens claras em caso de falha; confirmações antes de ações irreversíveis.
- **Flexibilidade e eficiência:** Histórico e timeline na Home permitem retomar trabalhos anteriores sem repetir todo o fluxo; atalhos visuais para as funções principais.
- **Redução de carga cognitiva:** Fluxo em etapas (wizard) em vez de muitas opções simultâneas; processamento técnico no backend, com foco da interface em visualização e decisão (Tópico 01, contexto de uso).

---

## Padrões de interface utilizados

| Padrão | Onde aparece | Justificativa |
|--------|--------------|---------------|
| **Wizard de múltiplos passos** | Fluxo Upload → Seleção de rede → Resultado | Divide a tarefa em etapas claras, reduzindo carga cognitiva e erros (Tópico 02: tendência de simplificação). |
| **Dashboard com widgets** | Tela Dashboard | Agrega estatísticas, gráficos e mapas em uma visão única; atende cenários de Insights e Comparação temporal (Tópico 04). |
| **Feedback de progresso** | Tela Upload (e durante processamento) | Comunica o estado do sistema (visibilidade do status); alinhado ao contexto de uso (Tópico 01). |
| **Master-detail / lista e detalhe** | Tela Seleção de rede | Lista de redes com detalhes (informações técnicas) ao selecionar; atende persona Dra. Helena (Tópico 03). |
| **Ponto de partida com histórico** | Home inicial | Timeline e histórico de uso; atende Cenário 5 – Histórico e timeline (Tópico 04). |

---

## Imagens das telas (design) e vínculo a personas e cenários

### Home inicial
![Home inicial](img/design/home_inicial.png)
- **Personas:** Ricardo Mendes, Felipe Antunes (acesso ao histórico e início de novo processamento).
- **Cenário (Tópico 04):** Cenário 5 – Histórico e timeline (Victor); também ponto de partida para Cenário 1 – Upload e segmentação (Vinicius).
- **Funcionalidade (Tópico 01):** Dashboard inicial (Histórico e timeline).

### Upload de imagem
![Upload de imagem](img/design/upload_imagem.png)
- **Personas:** Ricardo Mendes, Dra. Helena Silveira, Felipe Antunes.
- **Cenário (Tópico 04):** Cenário 1 – Upload e segmentação (Vinicius); início do fluxo do Cenário 2 (Gustavo).
- **Funcionalidade (Tópico 01):** Segmentação de imagens (upload).

### Seleção de rede
![Seleção de rede](img/design/seleção_rede.png)
- **Personas:** Dra. Helena Silveira (principal), Ricardo Mendes, Felipe Antunes.
- **Cenário (Tópico 04):** Cenário 2 – Seleção de modelo e validação técnica (Gustavo).
- **Funcionalidade (Tópico 01):** Seleção de redes neurais e informações técnicas.

### Dashboard
![Dashboard](img/design/dashboard.png)
- **Personas:** Ricardo Mendes, Cláudia Torres (insights e apresentação), Dra. Helena Silveira (métricas), Felipe Antunes (estatísticas e laudos).
- **Cenários (Tópico 04):** Cenário 3 – Insights e Dashboard (Deise); Cenário 4 – Comparação temporal (Lucas); Cenário 5 – Histórico e timeline (Victor).
- **Funcionalidade (Tópico 01):** Geração de insights e dashboards; Comparação temporal; visão consolidada do histórico.
