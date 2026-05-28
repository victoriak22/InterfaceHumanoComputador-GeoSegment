# Relatório Consolidado de Avaliação Heurística — GeoSegment

## 1. Introdução

O presente relatório apresenta os resultados da avaliação heurística realizada no sistema **GeoSegment**, plataforma desenvolvida para análise temporal e segmentação de imagens utilizando modelos de Inteligência Artificial.

O objetivo da avaliação foi identificar problemas de usabilidade presentes na interface do sistema, verificando sua aderência às heurísticas de usabilidade propostas por Jakob Nielsen e Rolf Molich. A avaliação buscou identificar dificuldades relacionadas à navegação, compreensão das funcionalidades, feedback visual, prevenção de erros e eficiência de uso.

A análise teve como foco principal:
- facilidade de uso;
- clareza da interface;
- eficiência das interações;
- consistência visual;
- suporte ao usuário;
- interpretação das informações apresentadas.

---

# 2. Método de Avaliação

Foi utilizado o método de **Avaliação Heurística**, baseado nas 10 heurísticas de usabilidade de Nielsen.

Cada avaliador realizou uma análise individual do sistema GeoSegment, identificando problemas de usabilidade, atribuindo níveis de severidade e propondo melhorias para os problemas encontrados.

As análises foram realizadas considerando as seguintes áreas do sistema:
- Home;
- Upload de imagens;
- Seleção de modelos;
- Comparação temporal;
- Histórico;
- Página “Sobre”.

---

# 3. Participantes da Avaliação

Participaram da avaliação heurística os seguintes especialistas:

- Deise Araujo
- Gustavo Dias Vicentin
- Lucas Rebolças
- Victor Iak
- Vinicius Saide

---

# 4. Interpretação dos Resultados

A interpretação dos resultados foi baseada na análise das avaliações individuais realizadas pelos especialistas, buscando identificar padrões recorrentes de problemas e tendências de usabilidade.

As avaliações demonstraram que o sistema GeoSegment possui:
- boa organização visual;
- identidade visual consistente;
- navegação relativamente intuitiva;
- estrutura moderna de interface.

Entretanto, foram identificados problemas recorrentes relacionados principalmente às seguintes heurísticas:

- Visibilidade do status do sistema;
- Compatibilidade entre sistema e mundo real;
- Reconhecimento em vez de memorização;
- Flexibilidade e eficiência de uso;
- Ajuda e documentação.

Os avaliadores observaram que usuários iniciantes podem apresentar dificuldades na compreensão:
- dos modelos de IA disponíveis;
- das métricas exibidas;
- dos gráficos comparativos;
- do fluxo completo das análises temporais.

Também foram identificadas limitações relacionadas à ausência de:
- feedback visual durante processamento;
- filtros inteligentes no histórico;
- mensagens contextualizadas de erro;
- ajuda contextual;
- documentação simplificada.

---

# 5. Consolidação dos Resultados

A consolidação interparticipante permitiu identificar problemas recorrentes encontrados por diferentes avaliadores.

Os principais problemas identificados em comum foram:

| Problema identificado | Frequência |
|---|---|
| Falta de feedback visual durante processamento | Muito recorrente |
| Ausência de explicações simples dos modelos | Muito recorrente |
| Falta de filtros no histórico | Recorrente |
| Excesso de informações em algumas telas | Recorrente |
| Ausência de ajuda contextual | Muito recorrente |
| Mensagens de erro pouco explicativas | Recorrente |
| Dificuldade para usuários iniciantes | Muito recorrente |

Os resultados demonstram forte convergência entre os avaliadores, aumentando a confiabilidade das observações registradas.

A consolidação também indicou que:
- os maiores problemas estão relacionados à experiência de usuários iniciantes;
- usuários experientes conseguem utilizar o sistema com maior facilidade;
- o sistema possui boa base visual, porém necessita melhorias de suporte e orientação.

---

# 6. Principais Problemas Encontrados

## 6.1 Visibilidade do Status do Sistema

Os avaliadores identificaram ausência de:
- barras de progresso;
- indicadores de carregamento;
- confirmação visual clara após upload;
- estimativa de tempo restante.

Isso gera sensação de travamento durante análises mais demoradas.

### Severidade predominante:
**Simples (2)**

---

## 6.2 Compatibilidade entre Sistema e Mundo Real

Os modelos “U-Net” e “DeepLabV3+” aparecem sem explicações simplificadas, dificultando compreensão por usuários sem experiência técnica.

Também foram observadas dificuldades na interpretação:
- de métricas ambientais;
- gráficos;
- indicadores temporais.

### Severidade predominante:
**Simples (2)** e **Grave (3)**

---

## 6.3 Liberdade e Controle do Usuário

Os avaliadores identificaram ausência de:
- cancelamento de análises;
- retorno rápido às configurações anteriores;
- reinício simplificado de novas comparações.

### Severidade predominante:
**Simples (2)**

---

## 6.4 Consistência e Padronização

Foram observadas pequenas diferenças entre:
- espaçamentos;
- tamanhos de botões;
- alinhamentos;
- componentes gráficos.

Apesar disso, a interface geral foi considerada consistente.

### Severidade predominante:
**Cosmético (1)**

---

## 6.5 Prevenção contra Erros

O sistema apresenta pouca prevenção antes de operações críticas, principalmente:
- upload de arquivos inválidos;
- análises iniciadas sem confirmação;
- ausência de limites claros de upload.

### Severidade predominante:
**Simples (2)**

---

## 6.6 Reconhecimento em vez de Memorização

Os usuários precisam memorizar:
- diferenças entre modelos;
- significado de métricas;
- funções específicas da interface.

A ausência de descrições resumidas aumenta a sobrecarga cognitiva.

### Severidade predominante:
**Simples (2)** e **Grave (3)**

---

## 6.7 Flexibilidade e Eficiência de Uso

O histórico não possui:
- filtros;
- pesquisa;
- organização inteligente.

Isso reduz eficiência principalmente para usuários frequentes.

### Severidade predominante:
**Simples (2)**

---

## 6.8 Projeto Minimalista e Estético

As telas de comparação temporal apresentam:
- muitos gráficos simultaneamente;
- excesso de métricas;
- sobrecarga visual em análises extensas.

### Severidade predominante:
**Simples (2)**

---

## 6.9 Recuperação de Erros

As mensagens de erro:
- são genéricas;
- utilizam alertas padrão;
- não explicam soluções;
- não auxiliam recuperação do problema.

### Severidade predominante:
**Cosmético (1)** e **Simples (2)**

---

## 6.10 Ajuda e Documentação

Foi identificada ausência de:
- tutorial inicial;
- onboarding;
- tooltips;
- ajuda contextual;
- documentação simplificada.

### Severidade predominante:
**Grave (3)**

---

# 7. Relato dos Resultados

Os resultados obtidos indicam tendências claras de problemas de usabilidade relacionados principalmente à orientação do usuário e ao suporte durante utilização do sistema.

Apesar de o GeoSegment apresentar:
- boa organização visual;
- interface moderna;
- consistência geral satisfatória;
- navegação relativamente intuitiva;

foram identificadas limitações importantes relacionadas à experiência de usuários iniciantes.

As avaliações demonstram que:
- o sistema possui boa estrutura funcional;
- existem oportunidades relevantes de melhoria;
- os problemas encontrados concentram-se principalmente em feedback, documentação e suporte ao usuário.

Também é importante destacar que os resultados da avaliação:
- indicam tendências de problemas;
- não representam garantia absoluta de ocorrência;
- dependem do contexto e perfil dos usuários avaliados.

---

# 8. Recomendações de Reprojeto

Com base nas análises realizadas, recomenda-se:

## Interface e Feedback
- adicionar barras de progresso;
- implementar indicadores de carregamento;
- mostrar confirmação visual após upload.

## Navegação e Eficiência
- criar filtros e pesquisa no histórico;
- melhorar navegação entre análises;
- permitir reinício rápido de comparações.

## Ajuda e Documentação
- criar onboarding inicial;
- adicionar tooltips;
- implementar ajuda contextual;
- simplificar explicações dos modelos.

## Mensagens de Erro
- criar mensagens personalizadas;
- explicar soluções possíveis;
- permitir nova tentativa rápida.

## Organização Visual
- reduzir excesso de informações simultâneas;
- dividir métricas em abas ou categorias;
- simplificar visualização de gráficos.

---

# 9. Conclusão

A avaliação heurística realizada no sistema GeoSegment permitiu identificar diversos aspectos positivos da interface, especialmente relacionados à organização visual, consistência geral e estrutura funcional da plataforma.

Entretanto, também foram encontrados problemas relevantes de usabilidade, principalmente associados:
- à ausência de feedback visual;
- à falta de ajuda contextual;
- à dificuldade de interpretação para usuários iniciantes;
- à pouca flexibilidade em algumas funcionalidades.

A consolidação das análises individuais mostrou forte recorrência entre os problemas identificados, demonstrando consistência nos resultados obtidos pelos avaliadores.

De forma geral, conclui-se que o sistema GeoSegment apresenta boa base de usabilidade, porém necessita melhorias relacionadas principalmente:
- ao suporte ao usuário;
- à documentação;
- à comunicação visual;
- à eficiência das interações.

---

# Referências

Molich, R., and Nielsen, J. (1990). *Improving a human-computer dialogue*. Communications of the ACM 33, 3 (March), 338–348.
