# COVID-19 Data Analysis 🦠

Este projeto apresenta uma Análise Exploratória de Dados (EDA) abrangente sobre a pandemia de COVID-19, utilizando conjuntos de dados públicos para entender a propagação do vírus, o impacto em diferentes países e as tendências ao longo do tempo.

## 📋 Descrição do Projeto
O notebook `covid-19-data-analysis.ipynb` processa e visualiza dados relacionados ao coronavírus (2019-nCoV), focando em métricas cruciais como número de casos confirmados, mortes, recuperações e casos ativos. A análise permite identificar os epicentros da pandemia e o comportamento do vírus em diferentes regiões da OMS.

## 🌍 Contexto
O conjunto de dados abrange informações desde o início da identificação do vírus em Wuhan, China. Ele inclui dados diários por país, dados agregados por região e estatísticas recentes (snapshot) fornecidas pelo Worldometer.

## 🎯 Objetivo
- Realizar a limpeza e preparação dos dados (tratamento de valores nulos).
- Identificar os países com os maiores números absolutos de casos, mortes e recuperações.
- Analisar a distribuição dos dados e correlações entre as variáveis.
- Visualizar a evolução temporal da pandemia.

## 🚀 Fluxo de Trabalho
1.  **Aquisição de Dados**: Download automático do dataset via API do Kaggle e extração dos arquivos ZIP.
2.  **Preparação dos Dados**:
    - Carregamento de múltiplos arquivos CSV (`country_wise_latest.csv`, `day_wise.csv`, etc.).
    - Inspeção de tipos de dados e identificação de valores ausentes.
    - Imputação de dados faltantes (ex: preenchimento com a mediana em colunas do Worldometer).
3.  **Análise Exploratória (EDA)**:
    - **Top 10 Países**: Gráficos de barras para identificar os países mais impactados em diferentes métricas.
    - **Distribuições**: Análise estatística das variáveis.
    - **Visual