# Definições Iniciais

## 1. Membros da Equipe

| Nome | RA |
|------|----| 
| **Deise Adriana Silva Araújo** | 22.222.024-6 |
| **Gustavo Dias Vicentin** | 22.123.061-8 |
| **Lucas Rebouças Silva** | 22.122.048-6 |
| **Victor Caldeira Iak** | 22.122.057-7 |
| **Vinicius Saidi Soares** | 22.122.064-3 |

## 2. Título Original do TCC

Segmentação Semântica por Aprendizado Profundo para Mapeamento de Uso e Cobertura do Solo

Título antigo: Ferramenta para Automatizar a Segmentação Semântica de Imagens Aéreas para Mapeamento Ambiental

## 3. Orientador(a)

Luciano Rossi <br>
lrossi@fei.edu.br

## 4. Desenvolvimento de Interface

- [X] Sim  
- [ ] Não  

## 5. Objetivo do Trabalho

O objetivo central é fornecer uma ferramenta de suporte à decisão e gestão territorial, tornando o processo de análise ambiental mais rápido, preciso e escalável do que o mapeamento manual tradicional

## 6. Produto Final

O produto final entregue é uma rede neural treinada para realizar o mapeamento (segmentação semântica) do uso e cobertura do solo, exposta em uma interface web intuitiva.

## 7. Usuário Final

Pesquisadores e especialistas ambientais.

## 8. Benefícios ao Usuário

- Agilidade no processo de segmentação;
- Confiabilidade dos resultados;
- Tomadas de decisões mais assertivas;

## 9. Funcionalidades da Ferramenta (Visão do Usuário)

Cada grande funcionalidade é de responsabilidade de um integrante da equipe e atende a uma ou mais personas (ver Tópico 03). Cada uma possui um cenário de análise de problemas no Tópico 04.

| # | Funcionalidade | Responsável | Persona(s) principal(is) | Cenário no Tópico 04 |
|---|----------------|-------------|---------------------------|----------------------|
| 1 | **Segmentação de imagens** – Upload e processamento de imagens (ex.: .tiff, .png) para segmentação semântica do uso e cobertura do solo | Vinicius Saidi Soares | Ricardo Mendes | Cenário 1 – Upload e segmentação |
| 2 | **Seleção de redes neurais e informações técnicas** – Escolha do modelo (ex.: U-Net, DeepLabV3+, LULC-SegNet) e exibição de qual rede está em uso, métricas e parâmetros | Gustavo Dias Vicentin | Dra. Helena Silveira | Cenário 2 – Seleção de modelo e validação técnica |
| 3 | **Geração de insights e painéis (dashboards)** – Análise da imagem segmentada, painéis com informações e características das áreas, gráficos e estatísticas por classe | Deise Adriana Silva Araújo | Ricardo Mendes, Cláudia Torres | Cenário 3 – Insights e Dashboard |
| 4 | **Comparação temporal de resultados** – Comparação entre períodos (ex.: ano atual vs. anterior), destaque de mudanças e variações por classe | Lucas Rebouças Silva | Ricardo Mendes, Felipe Antunes | Cenário 4 – Comparação temporal |
| 5 | **Dashboard inicial (Histórico e timeline)** – Acesso ao histórico de uso, timeline de processamentos e visão geral das atividades | Victor Caldeira Iak | Ricardo Mendes, Felipe Antunes | Cenário 5 – Histórico e timeline |

## 10. Tecnologias e Ferramentas Computacionais

- Linguagem de programação: Python
- Bibliotecas do Python: PyTorch, TensorFlow, Scikit-learn, entre outras
- Banco de dados: EM DISCUSSÃO
- Ferramentas de design e prototipação: Figma
- Redes neurais convolucionais: U-Net, DeepLabV3+ e LULC-SegNet
- Cronograma: Trello
- "Supercomputador Santos Dumont" do Laboratório Nacional de Computação Científica (LNCC)
- Artigo: OverLeaf

## 11. Contexto de Uso da Aplicação (IHC)

### Ambiente de utilização:
A aplicação será utilizada predominantemente em ambientes internos, como escritórios corporativos. Em casos específicos, poderá ser utilizada em ambientes rurais, desde que haja infraestrutura tecnológica disponível.

### Condições de uso:
O uso ocorre, em geral, em ambientes controlados, caracterizados por:

- Baixo nível de ruído
- Boa iluminação
- Ausência de vibrações ou movimentações intensas
- Postos de trabalho organizados (mesa, cadeira, monitor)

Em ambientes rurais, podem ocorrer variações como instabilidade de conexão ou iluminação.

### Dispositivos envolvidos:
- Computadores desktop
- Acesso à internet
- Navegadores web atualizados
- Teclado e mouse como principais dispositivos de entrada

### Limitações dos usuários:
Usuários com conhecimentos básicos a intermediários em informática

Possíveis limitações:

- Falta de conexão com a internet
- Quedas de energia
- Diferentes níveis de familiaridade com sistemas digitais

### Tipo de interação esperada:
Deslocar o controle técnico do usuário para o provedor de serviço, reduzindo a carga cognitiva e permitindo acesso rápido a análises complexas, com ênfase em visualização e interpretação de dados.

 **Interface Web Intuitiva:** acesso via navegador sem necessidade de instalação local.  
- **Interação Guiada por Filtros e Dashboards:** seleção de áreas de interesse, períodos temporais e categorias temáticas.  
- **Processamento Automatizado:** algoritmos de classificação, segmentação e análise preditiva operando no backend, invisíveis ao usuário.  
- **Feedback Visual Imediato:** mapas, gráficos e relatórios gerados em tempo real, com indicadores de qualidade e estatísticas resumidas.  
- **Minimização de Configuração Técnica:** o usuário foca na exploração de resultados e tomada de decisão, enquanto a infraestrutura gerencia processamento e armazenamento.  
- **Interação Orientada à Tarefa:** workflows simplificados que priorizam objetivos específicos (ex.: monitoramento de cobertura do solo, detecção de desmatamento, análise temporal de áreas protegidas).

Interação tradicional de desktop, baseada em:
- Interface gráfica (GUI)
- Uso de menus, botões e formulários
- Navegação por mouse e teclado
- Feedback visual imediato (mensagens, alertas, confirmações)

## 12. Critérios de Qualidade em IHC

O projeto busca alinhar a interface aos conceitos de qualidade em IHC abordados na disciplina (usabilidade, experiência do usuário, acessibilidade e comunicabilidade):

- **Usabilidade:** Eficácia (atingir objetivos de segmentação e análise), eficiência (reduzir tempo e esforço em relação a ferramentas manuais como QGIS) e satisfação do usuário (confiança e clareza no uso).
- **Experiência do usuário (UX):** Fluxos orientados à tarefa, feedback imediato e redução de carga cognitiva, de modo que analistas e gestores passem do resultado técnico à decisão de forma fluida.
- **Acessibilidade:** Contraste e legibilidade adequados, rótulos e textos compreensíveis e, onde aplicável, compatibilidade com boas práticas de acesso (ex.: alternativas textuais para mapas e gráficos em relatórios).
- **Comunicabilidade:** Mensagens do sistema claras (estado do processamento, erros, confirmações), linguagem adequada ao perfil do usuário (técnica para pesquisadores, mais direta para gestores) e feedback visual que comunique o estado atual da interface (visibilidade do status do sistema).

## 13. Matriz de rastreabilidade (Responsável × Funcionalidade × Cenário × Tela)

| Responsável | Funcionalidade | Persona(s) | Cenário (Tópico 04) | Tela(s) (Tópico 11) |
|-------------|----------------|------------|---------------------|---------------------|
| Vinicius Saidi Soares | Segmentação de imagens (upload) | Ricardo Mendes | Cenário 1 – Upload e segmentação | Home, Upload de imagem |
| Gustavo Dias Vicentin | Seleção de redes + informações técnicas | Dra. Helena Silveira | Cenário 2 – Seleção de modelo e validação técnica | Upload, Seleção de rede |
| Deise Adriana Silva Araújo | Insights e dashboards | Ricardo Mendes, Cláudia Torres | Cenário 3 – Insights e Dashboard | Dashboard |
| Lucas Rebouças Silva | Comparação temporal | Ricardo Mendes, Felipe Antunes | Cenário 4 – Comparação temporal | Dashboard |
| Victor Caldeira Iak | Dashboard inicial (Histórico e timeline) | Ricardo Mendes, Felipe Antunes | Cenário 5 – Histórico e timeline | Home, Dashboard |
