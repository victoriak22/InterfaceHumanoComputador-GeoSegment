# Tópico 08 - Processos de Projeto de IHC

Este documento apresenta uma análise dos **processos de projeto de Interação Humano-Computador (IHC)** aplicados ao desenvolvimento da plataforma *GeoSegment*, considerando tanto os aspectos técnicos quanto os princípios de design, restrições da plataforma e diretrizes externas que orientam sua construção.

---

## Introdução

O *GeoSegment* é uma aplicação web voltada ao mapeamento automático de uso e cobertura do solo em imagens aéreas de alta resolução. A plataforma adota o modelo *AIaaS* (*Artificial Intelligence as a Service*), disponibilizando inferência de segmentação semântica sob demanda por meio do navegador, sem a necessidade de instalação local ou conhecimento técnico avançado por parte do usuário.

Do ponto de vista de software, a solução é composta por:

- interface desenvolvida em **React com TypeScript**  
- backend implementado em **FastAPI (Python)**  
- modelo de aprendizado profundo baseado na arquitetura **DeepLabV3+**, com backbone **ResNet-101**, treinado com **PyTorch**  

O empacotamento da aplicação é realizado por meio de **Docker**, e o deploy ocorre na plataforma **Railway**.

No que se refere à infraestrutura de hardware:

- o treinamento do modelo foi realizado no supercomputador do **LNCC (Laboratório Nacional de Computação Científica)**  
- a inferência em produção ocorre nos servidores da Railway  
- o acesso é realizado via navegador, em qualquer dispositivo com conexão à internet  

---

## Capacidades e Restrições da Plataforma

A compreensão das capacidades e limitações da plataforma é fundamental para orientar decisões de projeto em IHC, uma vez que esses fatores impactam diretamente a experiência do usuário e as possibilidades de interação.

| **Capacidades** | **Restrições** |
|----------------|---------------|
| Acesso via navegador, sem necessidade de instalação local | Modelo treinado com apenas 35 imagens, limitando a generalização |
| Inferência automática em nível de pixel (8 classes) | Ausência de persistência de resultados |
| Geração de mapa temático com legenda padronizada | Ausência de comparação temporal |
| Exibição de proporções percentuais por classe | Limitação para imagens muito grandes (>2048×2048 px) |
| Arquitetura otimizada com menor latência | Ausência de autenticação de usuários |
| API RESTful em FastAPI, permitindo integração futura | Dependência da infraestrutura da Railway |
| Containerização via Docker (reprodutibilidade) | Exportação limitada (sem formatos georreferenciados) |
| Desempenho competitivo (73,81% mIoU) | Ausência de detecção automática de mudanças |
| Interface simples em tela única | Necessidade de conexão estável |

---

## Princípios Gerais de Projeto

O desenvolvimento do *GeoSegment* é orientado por princípios de projeto que consideram tanto o **contexto regulatório (aspecto de negócio)** quanto as **boas práticas de IHC e engenharia de software (aspecto de plataforma)**.

---

## Aspecto de Negócio

Esta seção apresenta normas, leis e regulamentações que orientam o domínio de aplicação do *GeoSegment*, especialmente no contexto de monitoramento ambiental e gestão territorial no Brasil.

### 1. Lei nº 9.985/2000 — Sistema Nacional de Unidades de Conservação (SNUC)

A lei que institui o SNUC estabelece critérios para criação e gestão de unidades de conservação, incluindo a APA de Petrópolis, área de estudo do projeto. O sistema prevê monitoramento contínuo e elaboração de planos de manejo baseados em dados territoriais atualizados.

Nesse contexto, o *GeoSegment* atua como ferramenta de apoio à geração desses dados.

Link: http://www.planalto.gov.br/ccivil_03/leis/l9985.htm

---

### 2. Resolução CONAMA nº 369/2006

Define condições para intervenções em áreas de preservação permanente. Os mapas gerados pelo *GeoSegment* podem servir como evidência técnica em processos de licenciamento e fiscalização.

Isso implica a necessidade de:

- precisão dos resultados  
- rastreabilidade  
- clareza na apresentação das informações  

Link: https://www.ibama.gov.br/component/legislacao/?view=legislacao&legislacao=93240

---

### 3. Política Nacional do Meio Ambiente — Lei nº 6.938/1981

Estabelece diretrizes para o monitoramento ambiental no Brasil e cria o SISNAMA. Essa legislação legitima o uso de ferramentas automatizadas como o *GeoSegment* no apoio a órgãos como o ICMBio.

Link: http://www.planalto.gov.br/ccivil_03/leis/l6938.htm

---

### 4. MapBiomas — Metodologia de Mapeamento de Uso e Cobertura do Solo

O MapBiomas é a principal referência nacional para classificação de uso e cobertura do solo. Sua taxonomia e metodologia orientam a evolução do *GeoSegment*, especialmente na definição de classes e padrões de análise.

Link: https://brasil.mapbiomas.org

---

## Aspecto de Plataforma

Esta seção apresenta diretrizes e boas práticas que orientam o design e a implementação da interface e da arquitetura do sistema.

### 1. Nielsen — 10 Heurísticas de Usabilidade

As heurísticas de Nielsen constituem um dos principais referenciais em IHC. No *GeoSegment*, destacam-se:

- visibilidade do estado do sistema (exibição de progresso)  
- correspondência com o mundo real (uso de termos compreensíveis)  
- controle e liberdade do usuário (possibilidade de refazer ações)  

Link: https://www.nngroup.com/articles/ten-usability-heuristics

---

### 2. W3C — Web Content Accessibility Guidelines (WCAG 2.1)

As diretrizes WCAG 2.1 estabelecem padrões de acessibilidade baseados em quatro princípios: perceptível, operável, compreensível e robusto.

No *GeoSegment*, são especialmente relevantes:

- contraste de cores  
- acessibilidade para usuários com daltonismo  
- navegação por teclado  

Link: https://www.w3.org/TR/WCAG21

---

### 3. Shneiderman — 8 Regras de Ouro

As regras de Shneiderman reforçam princípios como:

- consistência  
- feedback informativo  
- prevenção e tratamento de erros  

Aplicações no *GeoSegment* incluem:

- exibição de progresso da segmentação  
- confirmação visual de sucesso  
- mensagens claras de erro  

Link: https://www.cs.umd.edu/users/ben/goldenrules.html

---

### 4. React — Boas Práticas de Desenvolvimento

A documentação do React orienta padrões de:

- componentização  
- gerenciamento de estado  
- organização do código  

Esses aspectos são fundamentais para garantir a escalabilidade da interface do *GeoSegment*.

Link: https://react.dev

---

### 5. FastAPI — Boas Práticas de API REST

O FastAPI segue padrões OpenAPI e boas práticas RESTful, permitindo:

- documentação automática  
- integração com outros sistemas  
- manutenção facilitada  

Link: https://fastapi.tiangolo.com

---

## Considerações Finais

A análise evidencia que o projeto do *GeoSegment* está fundamentado em princípios sólidos de IHC, alinhados tanto ao contexto regulatório quanto às boas práticas de desenvolvimento e design de interfaces.

A integração entre capacidades técnicas, restrições da plataforma e diretrizes externas contribui para a construção de uma solução coerente, escalável e orientada às necessidades reais dos usuários no domínio ambiental.

---

## Metas de Usabilidade

As metas de usabilidade do *GeoSegment* foram definidas com base na proposta de **Nielsen (1993)**, que estrutura a usabilidade em cinco atributos mensuráveis, e no ciclo de engenharia de usabilidade de **Mayhew (1999)**, que orienta a definição de metas quantitativas e qualitativas alinhadas ao perfil dos usuários e às tarefas principais do sistema.

As tarefas consideradas como referência são as três ações centrais da ferramenta:

- envio de imagem aérea  
- geração do mapa segmentado  
- leitura das proporções por classe  

---

### 1. Facilidade de Aprendizado (*Learnability*)

#### Análise qualitativa

O *GeoSegment* deve ser utilizável por analistas ambientais e gestores territoriais que não necessariamente possuem formação em computação ou experiência com ferramentas de aprendizado de máquina. Nesse contexto, a interface deve ser autoexplicativa, permitindo que o usuário compreenda o fluxo de uso sem necessidade de treinamento prévio.

O fluxo principal — envio da imagem, processamento e visualização do resultado — deve ser apresentado de forma linear e intuitiva, com elementos visuais que orientem claramente cada etapa.

#### Meta quantitativa

- Um usuário sem experiência prévia deve ser capaz de completar o fluxo completo em até **3 minutos**, sem auxílio externo.

---

### 2. Eficiência de Uso (*Efficiency*)

#### Análise qualitativa

Para usuários recorrentes, como analistas que realizam monitoramentos periódicos, a interface não deve introduzir fricção no fluxo de trabalho. A eficiência está relacionada ao tempo necessário para executar ações na interface, e não ao tempo de processamento do modelo.

Elementos como localização de comandos, visibilidade de resultados e organização da informação devem permitir execução rápida das tarefas.

#### Meta quantitativa

- Um usuário experiente deve completar o fluxo completo em até **1 minuto**, desconsiderando o tempo de processamento no servidor.  
- O mapa segmentado e as proporções por classe devem estar visíveis na **mesma tela**, sem necessidade de navegação adicional.

---

### 3. Facilidade de Memorização (*Memorability*)

#### Análise qualitativa

Considerando o uso intermitente da ferramenta, a interface deve permitir que o usuário retome sua utilização sem necessidade de reaprendizado. A consistência visual, especialmente na representação das classes, é essencial para esse objetivo.

A paleta de cores adotada deve ser intuitiva e semanticamente coerente (por exemplo, verde para vegetação e azul para água), reduzindo a dependência de consulta à legenda.

#### Meta quantitativa

- Um usuário que não acessa a ferramenta há **30 dias** deve ser capaz de retomar o fluxo completo em até **2 minutos**, sem suporte externo.  
- A legenda de cores deve ser corretamente interpretada em pelo menos **80% dos casos** em testes de memória.

---

### 4. Tolerância a Erros (*Error Rate*)

#### Análise qualitativa

Os principais erros esperados envolvem:

- envio de arquivos em formato incompatível  
- imagens com resolução inadequada  
- tentativas de processamento de arquivos acima da capacidade da plataforma  

A interface deve fornecer mensagens claras, orientadas à ação, evitando termos técnicos ou mensagens de erro internas (como códigos HTTP ou stack traces).

#### Meta quantitativa

- Mensagens de erro devem ser exibidas em até **3 segundos** após a ocorrência.  
- A taxa de erros não recuperados deve ser inferior a **10%** em testes com usuários reais.

---

### 5. Satisfação Subjetiva (*Satisfaction*)

#### Análise qualitativa

A satisfação do usuário está diretamente relacionada à confiança nos resultados gerados pela ferramenta. Para isso, a interface deve:

- apresentar métricas de desempenho de forma acessível  
- permitir comparação visual entre imagem original e resultado segmentado  
- evitar terminologia excessivamente técnica  

Esses elementos contribuem para a percepção de confiabilidade e utilidade da ferramenta no apoio à tomada de decisão.

#### Meta quantitativa

- Ao menos **75% dos usuários** devem avaliar a ferramenta com nota ≥ 4 (em escala de 1 a 5) em critérios de clareza, confiança e facilidade de uso.  
- A pontuação mínima aceitável no **SUS (System Usability Scale)** é de **70 pontos**.
