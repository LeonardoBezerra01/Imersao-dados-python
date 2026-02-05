# 📊 Dashboard de Salários na Área de Dados

Este projeto é uma aplicação web interativa desenvolvida em Python para análise exploratória de dados salariais de profissionais da área de dados (Data Science, Data Engineering, Analytics, etc.) ao redor do mundo.

O dashboard permite filtrar informações por ano, nível de experiência e tipo de contrato, oferecendo visualizações gráficas sobre distribuição salarial, modalidades de trabalho e localização geográfica.

## 📋 Índice

- [Visão Geral](#visão-geral)
- [Pré-requisitos](#pré-requisitos)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Funcionalidades](#funcionalidades)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Dicionário de Dados](#dicionário-de-dados)
- [Instalação e Execução](#instalação-e-execução)
- [Contribuição](#contribuição)


---

## Visão Geral

A aplicação consome uma base de dados histórica de salários e utiliza a biblioteca **Streamlit** para criar uma interface amigável. O objetivo é responder perguntas como:
* Qual a média salarial por senioridade?
* Quais os cargos com maiores remunerações?
* Qual a proporção entre trabalho remoto e presencial?
* Como os salários de Cientistas de Dados variam por país?

---

## Pré-requisitos

Para executar este projeto, é necessário ter instalado em sua máquina:
* Python 3.8 ou superior.
* Gerenciador de pacotes pip.

---

## Tecnologias Utilizadas

O projeto foi construído com as seguintes bibliotecas Python:

* **[Streamlit](https://streamlit.io/):** Framework para construção do dashboard web.
* **[Pandas](https://pandas.pydata.org/):** Leitura, limpeza e manipulação dos dados.
* **[Plotly Express](https://plotly.com/python/plotly-express/):** Criação de gráficos interativos e mapas.

---

## Funcionalidades

O dashboard é dividido em três seções principais de interação:

### 1. Barra Lateral (Filtros)
Permite ao usuário refinar os dados exibidos nos gráficos através de seleção múltipla. As opções são carregadas dinamicamente com base no dataset:
* **Ano:** Seleção dos anos de referência.
* **Senioridade:** Filtragem por nível (Junior, Pleno, Senior, Executive).
* **Tipo de Contrato:** Filtragem por modalidade (Full-time, Freelance, etc.).

### 2. Métricas Gerais (KPIs)
Exibidas no topo da página principal, refletindo instantaneamente os filtros aplicados:
* **Total de Registros:** Volume de dados sendo analisados.
* **Média Salarial (USD):** Média anual dos salários convertida para Dólares.
* **Maior Salário (USD):** O teto salarial encontrado na seleção atual.

### 3. Visualizações Gráficas
* **Média Salarial por Senioridade (Gráfico de Barras):** Compara a remuneração média entre os diferentes níveis de experiência.
* **Média Salarial por Cargo (Gráfico de Barras):** Ranking dos cargos com maiores médias salariais (Top 10 ou geral).
* **Proporção dos Tipos de Trabalho (Gráfico de Rosca):** Distribuição percentual entre as modalidades (Remoto, Presencial, Híbrido).
* **Mapa Global de Salários (Mapa Coroplético):** Focado no cargo de **Data Scientist**, colore os países baseando-se na média salarial em USD, utilizando códigos ISO3 para geolocalização precisa.

---

## Estrutura do Projeto

```text
/
├── app.py                   # Código principal da aplicação (Dashboard)
├── dados-imersao-final.csv  # Base de dados (CSV)
└── requirements.txt         # Lista de dependências do Python
```

---

## Dicionário de Dados

A base de dados (dados-imersao-final.csv) contém as seguintes colunas utilizadas na análise:

---

## Instalação e execução

---

## Contribuição

---

