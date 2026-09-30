# 📊 Análise de Cancelamento de Clientes com Python

## Sobre o projeto

Este projeto foi desenvolvido como uma prática de **análise de dados utilizando Python**, com foco na identificação de padrões relacionados ao cancelamento de clientes.

A atividade utiliza uma base de dados com **50.000 registros e 11 variáveis**, contendo informações como idade, frequência de uso, quantidade de ligações para o call center, dias de atraso, tipo de assinatura, duração do contrato, total gasto e meses desde a última interação.

O objetivo da análise foi explorar a base de dados, realizar o tratamento das informações e identificar possíveis fatores relacionados ao cancelamento de clientes.

## 🛠️ Tecnologias utilizadas

* **Python**
* **Pandas** — leitura, tratamento e análise dos dados
* **Plotly** — criação de visualizações e gráficos
* **Jupyter Notebook** — desenvolvimento e documentação da análise
* **CSV** — formato utilizado para armazenamento da base de dados

## 🔎 Etapas realizadas

### 1. Importação dos dados

A base de dados foi carregada utilizando o Pandas:

```python
import pandas as pd

tabela = pd.read_csv("cancelamentos.csv")
```

### 2. Tratamento dos dados

Foram realizadas verificações iniciais para entender a estrutura da base e identificar possíveis problemas.

Entre os tratamentos realizados estão:

* Remoção da coluna `CustomerID`;
* Verificação das informações e tipos das colunas;
* Identificação de valores vazios;
* Remoção de registros com informações ausentes.

### 3. Análise inicial

Foi analisada a coluna `cancelou` para identificar:

* Quantidade de clientes que cancelaram;
* Quantidade de clientes que permaneceram;
* Proporção de cancelamentos na base.

Na base analisada, aproximadamente **56,8% dos registros correspondem a clientes que cancelaram** após o tratamento dos dados.

### 4. Análise exploratória

Foram utilizados gráficos com **Plotly** para observar a relação entre o cancelamento e as diferentes variáveis disponíveis na base.

A análise considerou características como:

* Idade;
* Sexo;
* Tempo como cliente;
* Frequência de uso;
* Ligações para o call center;
* Dias de atraso;
* Tipo de assinatura;
* Duração do contrato;
* Total gasto;
* Tempo desde a última interação.

### 5. Análise de possíveis fatores

Após a análise inicial, foram realizados filtros para observar como determinados critérios alteravam a proporção de cancelamentos.

Foram avaliados, entre outros pontos:

* Clientes com contratos diferentes do mensal;
* Clientes com até 4 ligações para o call center;
* Clientes com até 20 dias de atraso.

Esses filtros foram utilizados como uma forma de explorar possíveis estratégias para redução de cancelamentos.

## 📁 Arquivos

```text
├── README.md
├── cancelamentos.csv
└── inicial.ipynb
```

## 🎯 Objetivo de aprendizado

O principal objetivo deste projeto foi praticar um fluxo básico de análise de dados utilizando Python:

**Importação → Tratamento → Exploração → Visualização → Análise**

Este projeto faz parte dos meus estudos em Python e representa uma aplicação prática dos conhecimentos iniciais de **Pandas e análise de dados**.

## 🚀 Próximos passos

Como evolução deste projeto, algumas possibilidades seriam:

* Criar uma análise mais aprofundada dos fatores de cancelamento;
* Melhorar as visualizações;
* Criar um dashboard interativo utilizando **Streamlit**;
* Explorar correlações entre as variáveis;
* Desenvolver novas métricas para acompanhamento dos cancelamentos.

