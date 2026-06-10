# Estratégia de Retenção de Clientes e Predição de Churn: Model Fitness

## Descrição do Projeto
Este projeto foi desenvolvido com foco em Inteligência de Negócios e Análise de Sobrevivência de Clientes para a rede de academias Model Fitness. O desafio consistiu em transformar dados comportamentais e demográficos em uma estratégia eficiente de combate ao *churn* (cancelamento de planos). A análise envolveu uma profunda Análise Exploratória de Dados (EDA), mapeamento de perfis de comportamento via segmentação analítica, formulação de hipóteses e a proposição de ações de marketing preditivas e direcionadas para mitigar a perda de receita e aumentar o *Lifetime Value* (LTV) dos clientes.

---

## Tecnologias e Ferramentas Utilizadas
* **Linguagem:** Python
* **Análise e Manipulação de Dados:** Pandas e NumPy
* **Visualização de Dados e Gráficos Estáticos:** Matplotlib e Seaborn
* **Ambiente de Desenvolvimento:** Jupyter Notebook

---

## Pipeline de Dados e Metodologia

### 1. Auditoria e Consistência da Base de Dados
* Carga e inspeção de uma base de dados contendo o histórico de 4.000 clientes e 14 variáveis (atributos demográficos e de engajamento).
* Diagnóstico de integridade da base, confirmando a ausência de valores ausentes (nulos) ou duplicados, garantindo a confiabilidade estatística para as etapas de modelagem subsequentes.

### 2. Análise Exploratória de Dados (EDA) e Perfilamento Comportamental
* Segmentação e agrupamento da base de dados com foco na variável alvo (`Churn`), calculando as médias e distribuições de cada atributo para entender quem é o cliente que sai vs. o cliente que permanece.
* Identificação de correlações e padrões de comportamento, avaliando o impacto de fatores como proximidade física da unidade, uso de cupons de parceiros (`Promo_friends`) e gastos em serviços adicionais.

### 3. Análise Visual de Distribuição de Variáveis
* Construção de histogramas de distribuição e gráficos de barra contrastando diretamente os clientes ativos contra os que deram *churn*.
* Avaliação visual do comportamento de variáveis contínuas (como idade, gastos adicionais e frequência de treinos) para isolar visualmente os pontos de virada (*turning points*) onde o risco de cancelamento aumenta.

---

## Principais Insights & Impacto de Negócio
* **O Fator Tempo (Fricção Inicial):** O principal indicador de *churn* é o tempo de casa (*Lifetime*). Clientes nos primeiros dois meses apresentam um risco criticamente elevado de cancelamento, tornando as primeiras 8 semanas o período de ouro para ações de engajamento.
* **Frequência de Treino Prova o Risco:** Alunos que treinam menos de 2 vezes por semana entram em uma zona de perigo iminente. A queda na média semanal atual em relação à média histórica serve como um termômetro preditivo claro para o negócio agir antes do cancelamento formal.
* **O Poder do Vínculo Social e Comercial:** Clientes que aderiram por indicação de amigos (`Promo_friends`) ou que possuem contratos de longo prazo (6 a 12 meses) apresentam taxas de *churn* drasticamente menores, provando que a estabilidade contratual e o senso de comunidade blindam a receita.
* **Gatilhamento de Marketing Direto:** Recomenda-se a implementação de um alerta automatizado na catraca quando a frequência do aluno cair. Isso dispara um gatilho para o envio de mensagens de acolhimento e o agendamento de uma reavaliação física gratuita, trazendo o aluno de volta à rotina.
* **Estratégia de Aquisição Inteligente:** O negócio deve desencorajar a adesão cega a planos mensais curtos, transformando os pacotes semestrais e anuais nas opções financeiramente mais inteligentes através de descontos agressivos na matrícula ou isenção de taxas condicionada ao cadastro completo dos dados.

---

