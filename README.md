# Análise da Arrecadação Tributária Estadual (ICMS, IPVA e Outros)

## Visão Geral do Projeto

Este projeto consiste em uma **análise exploratória de dados (Exploratory Data Analyse)** da arrecadação de tributos estaduais (principalmente ICMS, IPVA, ITCD e Taxas) dos estados brasileiros ao longo do tempo. O objetivo é identificar as principais **tendências temporais**, o **ranking de arrecadação** por estado e o **DNA fiscal** de cada região, ou seja, de quais setores econômicos sua receita é mais dependente.

O código foi desenvolvido em um *notebook* Jupyter (`arrecadacao_estados.ipynb`) e utiliza as bibliotecas `pandas`, `matplotlib` e `seaborn` para manipulação, agrupamento e visualização dos dados.

## Análises Chave Realizadas

O projeto aborda as seguintes perspectivas de análise:

1.  **Evolução Temporal Global:** Visualização da Receita Tributária Total (soma de todos os estados) desde 1997 para identificar tendências de crescimento e sazonalidade.
2.  **Ranking Regional Acumulado:** Classificação dos estados pela Receita Tributária Total acumulada, destacando a alta concentração de arrecadação nos principais polos econômicos.
3.  **Composição Setorial do ICMS (Top 10):** Análise da matriz fiscal de ICMS, mostrando a proporção da receita que vem do setor **Primário**, **Secundário**, **Terciário**, **Energia Elétrica** e **Combustíveis**.
4.  **Composição de Outros Tributos (Top 10):** Detalhamento da arrecadação de **IPVA**, **ITCD** e **Taxas** por estado.

## Tecnologias Utilizadas

* **Python:** Linguagem principal do projeto.
* **`pandas`:** Essencial para leitura (`.read_excel`), manipulação, limpeza (`.dropna()`) e agrupamento (`.groupby()`) dos dados.
* **`matplotlib` & `seaborn`:** Utilizadas para a criação dos gráficos de linha, ranking de barras e barras empilhadas.
* **`numpy`:** Usado para operações numéricas.
* **`scikit-learn` (Opcional):** Embora importada, a biblioteca `sklearn` (originalmente para `LabelEncoder`) não foi utilizada na análise final, mas está presente no *notebook* inicial.

## Como Executar o Projeto

Para replicar a análise, siga os passos abaixo:

### 1. Pré-requisitos

Certifique-se de ter o Python (versão 3.12.2) e o `pip` instalados.

### 2. Instalação das Bibliotecas

Execute o comando no seu terminal ou na primeira célula do Jupyter:

```bash
pip install pandas matplotlib seaborn openpyxl
