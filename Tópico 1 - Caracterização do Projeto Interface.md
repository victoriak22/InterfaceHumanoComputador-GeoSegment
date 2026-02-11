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

- Segmentar imagens (ex.: .tiff ou .png)
- Seleção de redes neurais
- Informações técnicas (ex.: qual rede neural está sendo utilizada)
- Geração de insights sobre a imagem segmentada da área
- Painéis e dashboards que mostram informações e características das áreas segmentadas
- Comparação temporal de resultados

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
Interação tradicional de desktop, baseada em:

- Interface gráfica (GUI)
- Uso de menus, botões e formulários
- Navegação por mouse e teclado
- Feedback visual imediato (mensagens, alertas, confirmações)
