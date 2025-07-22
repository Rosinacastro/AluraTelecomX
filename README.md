# 📊 Análise de Evasão de Clientes (Churn Analysis)

Este projeto tem como objetivo identificar padrões e possíveis causas para a evasão de clientes (*churn*) em uma base de dados da empresa de telecomunicação Telecom X. A análise foi conduzida por meio de limpeza, visualização de dados e engenharia de atributos, com o objetivo de gerar insights que orientem estratégias de retenção.

---

## 🧠 Objetivos

- Compreender o comportamento dos clientes que cancelaram o serviço.
- Identificar variáveis com maior impacto no churn.
- Gerar insights que auxiliem na tomada de decisões estratégicas.

---

## 📂 Estrutura do Projeto

```
📁 projeto-churn/
├── data/                # Conjunto de dados original e processado
├── notebooks/           # Jupyter Notebooks com todas as análises
├── imgs/                # Gráficos gerados na análise
├── README.md            # Este arquivo
└── requirements.txt     # Dependências do projeto
```

---

## 🔧 Tecnologias Utilizadas

- Python 3.11
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📌 Principais Etapas

### 🔹 1. Importação e Tratamento dos Dados

- Leitura de arquivos JSON com dados aninhados.
- Normalização e transformação de colunas.
- Conversão de colunas categóricas e numéricas para tipos apropriados.
- Tratamento de valores ausentes e inconsistências.

### 🔹 2. Análise Exploratória

- Análise descritiva com média, mediana, desvio padrão.
- Gráficos de distribuição de churn por variáveis categóricas (gênero, contrato, método de pagamento).
- Análise de variáveis numéricas como gasto total e tempo de contrato.

### 🔹 3. Engenharia de Atributos

- Criação da coluna `Contas_Diarias` a partir do faturamento mensal.
- Transformação de colunas "Sim"/"Não" para valores binários (1 e 0).
- Conversão da variável `Churn` para formato binário (0 = Não, 1 = Sim).

### 🔹 4. Geração de Insights

- Identificação de padrões de churn por tipo de contrato, tempo de permanência e uso de serviços.
- Avaliação do impacto do método de pagamento e serviços adicionais.

---

## ✅ Conclusões e Insights

- ⏱️ **Tempo de permanência (tenure)** é um forte preditor de churn: quanto menor o tempo, maior a evasão.
- 📄 **Tipo de contrato** é determinante: contratos de longo prazo tendem a reter mais clientes.
- 🔐 **Clientes que utilizam menos serviços adicionais**, como segurança digital, tendem a cancelar mais.
- 💳 **Pagamento automático** pode estar associado a clientes menos engajados.

---

## 💡 Recomendações

Com base nas análises, sugerem-se as seguintes ações:

- 🎯 Incentivar contratos anuais ou bianuais com descontos progressivos.
- 📦 Oferecer pacotes com serviços adicionais incluídos, como backup e segurança online.
- 👋 Melhorar o onboarding nos primeiros meses do cliente, período com maior risco de churn.
- 📉 Acompanhar de perto clientes com baixo tempo de permanência e baixo gasto total, com estratégias de fidelização.
- 🔍 Analisar o perfil dos clientes que utilizam pagamento automático, pois esse grupo apresenta alta evasão.

---

## 🧪 Passo Adicional: Análise de Correlação

Exploramos a correlação entre:

- A **conta diária** e a evasão.
- A **quantidade de serviços contratados** e a probabilidade de churn.

Essas análises indicam que quanto mais serviços contratados e maior o valor investido por dia, menor a evasão.

---

## 👩‍💻 Criado por

Rosina Castro  
[![GitHub](https://img.shields.io/badge/GitHub-rosinacastro-blue?logo=github)](https://github.com/rosinacastro)  
✨ *"Where code meets insight."*

---

## 📌 Licença

Este projeto é de uso educacional e está aberto para contribuições.
