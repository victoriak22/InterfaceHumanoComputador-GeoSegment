# Tópico 08 - Processos de Projeto de IHC

Este documento apresenta uma análise dos **processos de projeto de Interação Humano-Computador (IHC)** aplicados ao desenvolvimento da plataforma *GeoSegment*, incluindo a compreensão do contexto tecnológico, a adoção de diretrizes de design e a definição de metas de usabilidade que orientam a construção da interface.

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

A compreensão das capacidades e limitações da plataforma é fundamental para orientar decisões de projeto em IHC, uma vez que esses fatores impactam diretamente a experiência do usuário e as possibilidades de interação. Esses aspectos servem como base para a definição dos princípios de design adotados no sistema.

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

Com base nas capacidades e restrições identificadas, o desenvolvimento do *GeoSegment* é orientado por princípios de projeto que consideram tanto o **contexto regulatório (aspecto de negócio)** quanto as **boas práticas de IHC e engenharia de software (aspecto de plataforma)**.

---

## Aspecto de Negócio

Esta seção apresenta normas, leis e regulamentações que orientam o domínio de aplicação do *GeoSegment*, especialmente no contexto de monitoramento ambiental e gestão territorial no Brasil.

### 1. Lei nº 9.985/2000 - Sistema Nacional de Unidades de Conservação (SNUC)

A lei que institui o SNUC estabelece critérios para criação e gestão de unidades de conservação, incluindo a APA de Petrópolis, área de estudo do projeto. O sistema prevê monitoramento contínuo e elaboração de planos de manejo baseados em dados territoriais atualizados.

Nesse contexto, o *GeoSegment* atua como ferramenta de apoio à geração desses dados.

Link: http://www.planalto.gov.br/ccivil_03/leis/l9985.htm

---

### 2. Resolução CONAMA nº 369/2006

Define condições para intervenções em áreas de preservação permanente. Os mapas gerados pelo *GeoSegment* podem ser utilizados como evidência técnica em processos de licenciamento e fiscalização.

Isso implica a necessidade de:

- precisão dos resultados  
- rastreabilidade  
- clareza na apresentação das informações  

Link: https://www.ibama.gov.br/component/legislacao/?view=legislacao&legislacao=93240

---

### 3. Política Nacional do Meio Ambiente - Lei nº 6.938/1981

Estabelece diretrizes para o monitoramento ambiental no Brasil e cria o SISNAMA. Essa legislação legitima o uso de ferramentas automatizadas como o *GeoSegment* no apoio a órgãos como o ICMBio.

Link: http://www.planalto.gov.br/ccivil_03/leis/l6938.htm

---

### 4. MapBiomas - Metodologia de Mapeamento de Uso e Cobertura do Solo

O MapBiomas constitui a principal referência nacional para classificação de uso e cobertura do solo. Sua taxonomia e metodologia orientam a evolução do *GeoSegment*, especialmente na definição de classes e padrões de análise adotados pela interface.

Link: https://brasil.mapbiomas.org

---

## Aspecto de Plataforma

Considerando o contexto apresentado, o projeto da interface e da arquitetura do sistema segue diretrizes consolidadas na área de IHC e desenvolvimento web.

### 1. Nielsen - 10 Heurísticas de Usabilidade

As heurísticas de Nielsen constituem um dos principais referenciais em IHC. No *GeoSegment*, destacam-se:

- visibilidade do estado do sistema (exibição de progresso durante a segmentação)  
- correspondência com o mundo real (uso de termos como “vegetação” e “área urbana”)  
- controle e liberdade do usuário (possibilidade de reenviar imagens)  

Link: https://www.nngroup.com/articles/ten-usability-heuristics

---

### 2. W3C - Web Content Accessibility Guidelines (WCAG 2.1)

As diretrizes WCAG 2.1 estabelecem padrões de acessibilidade baseados nos princípios perceptível, operável, compreensível e robusto.

No *GeoSegment*, esses princípios impactam diretamente:

- a escolha da paleta de cores utilizada na representação das classes  
- a distinção visual para usuários com daltonismo  
- a navegação por teclado  

Link: https://www.w3.org/TR/WCAG21

---

### 3. Shneiderman - 8 Regras de Ouro

As regras de Shneiderman reforçam princípios como consistência, feedback e prevenção de erros.

Aplicações no *GeoSegment* incluem:

- exibição de progresso durante o processamento  
- confirmação visual de conclusão da tarefa  
- mensagens de erro claras e orientadas à ação  

Link: https://www.cs.umd.edu/users/ben/goldenrules.html

---

### 4. React - Boas Práticas de Desenvolvimento

A documentação do React orienta padrões de componentização, gerenciamento de estado e organização do código, fundamentais para garantir a escalabilidade da interface frente à evolução do sistema.

Link: https://react.dev

---

### 5. FastAPI - Boas Práticas de API REST

O FastAPI segue padrões OpenAPI e boas práticas RESTful, permitindo documentação automática, integração com outros sistemas e manutenção facilitada da API.

Link: https://fastapi.tiangolo.com

---

## Metas de Usabilidade

Com base nos princípios apresentados, são definidas metas de usabilidade mensuráveis, alinhadas às tarefas centrais do sistema e ao perfil dos usuários.

As metas são fundamentadas na proposta de **Nielsen (1993)** e no ciclo de engenharia de usabilidade de **Mayhew (1999)**.

As tarefas consideradas como referência são:

- envio de imagem aérea  
- geração do mapa segmentado  
- leitura das proporções por classe  

---

### 1. Facilidade de Aprendizado (*Learnability*)

#### Análise qualitativa

O *GeoSegment* deve ser utilizável por analistas ambientais e gestores territoriais que não necessariamente possuem formação em computação. A interface deve ser autoexplicativa e permitir compreensão imediata do fluxo de uso.

#### Meta quantitativa

- Completar o fluxo em até **3 minutos**, sem auxílio.

---

### 2. Eficiência de Uso (*Efficiency*)

#### Meta quantitativa

- Completar o fluxo em até **1 minuto** (sem processamento).  
- Informações visíveis na mesma tela.

---

### 3. Memorização (*Memorability*)

#### Meta quantitativa

- Retomar uso em até **2 minutos** após 30 dias.  
- 80% de reconhecimento das cores.

---

### 4. Tolerância a Erros

#### Meta quantitativa

- Erros exibidos em até **3 segundos**.  
- Menos de **10% de abandono**.

---

### 5. Satisfação

#### Meta quantitativa

- 75% com nota ≥ 4  
- SUS ≥ 70

---

## Avaliação das Metas

As metas serão avaliadas por meio de:

- testes com usuários reais  
- cronometragem de tarefas  
- observação direta  
- aplicação do SUS  

---

## Considerações Finais

A análise evidencia que o projeto do *GeoSegment* está fundamentado em princípios sólidos de IHC, alinhados tanto ao contexto regulatório quanto às boas práticas de desenvolvimento e design de interfaces.

A integração entre capacidades técnicas, restrições da plataforma, diretrizes de projeto e metas de usabilidade contribui para a construção de uma solução coerente, escalável e orientada às necessidades reais dos usuários no domínio ambiental.
