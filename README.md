# Projeto de Análise de Cancelamento de Clientes (Churn)

Este projeto tem como objetivo realizar uma análise exploratória de dados para compreender o comportamento dos clientes e identificar os principais motivos que levam ao cancelamento de subscrições (Churn). Todo o código e o desenvolvimento passo a passo encontram-se no ficheiro principal do projeto: **"Análise de dados.ipynb"**.

## 📊 Sobre os Dados

A análise utiliza como fonte de dados o ficheiro `cancelamentos.csv`. A base de dados contém as seguintes informações dos clientes:
* `idade`
* `sexo`
* `tempo_como_cliente`
* `frequencia_uso`
* `ligacoes_callcenter`
* `dias_atraso`
* `assinatura`
* `duracao_contrato`
* `total_gasto`
* `meses_ultima_interacao`
* `cancelou` (Variável alvo)

## ⚙️ Funcionalidades e Etapas da Análise

O desenvolvimento no ficheiro "Análise de dados.ipynb" foi dividido nas seguintes etapas lógicas:

1. **Importação de Dados:** Leitura do ficheiro CSV utilizando a biblioteca Pandas.
2. **Visualização Inicial e Limpeza:** Remoção de colunas que não agregam valor à análise (como o `CustomerID`) para evitar ruído nos dados.
3. **Tratamento de Dados:** Verificação da integridade dos dados e remoção de linhas que continham valores nulos ou vazios (`dropna`).
4. **Análise Inicial de Churn:** Verificou-se, de forma preliminar, que o cenário conta com uma taxa de cancelamento de **56.79%**, contra **43.21%** de clientes ativos.
5. **Análise Gráfica:** Utilização da biblioteca Plotly para gerar histogramas interativos, cruzando as várias características dos clientes (como a `idade`) com o estado de cancelamento, de forma a extrair insights e padrões.

## 🛠️ Tecnologias Utilizadas

Para executar este projeto, foram utilizadas as seguintes ferramentas e bibliotecas em Python:
* **Pandas:** Para manipulação, tratamento e análise das estruturas de dados.
* **Plotly:** Para a criação de gráficos interativos e visualização de dados avançada.
* **Jupyter Notebook:** O ambiente interativo utilizado no desenvolvimento ("Análise de dados.ipynb").

## 🚀 Como Executar o Projeto

1. Certifique-se de ter o Python instalado no seu computador.
2. Instale as dependências necessárias através do terminal:
   ```bash
   pip install pandas plotly jupyter
   ```
3. Garanta que o ficheiro da base de dados (`cancelamentos.csv`) está na mesma pasta do código.
4. Inicie o Jupyter e abra o arquivo **"Análise de dados.ipynb"**.
5. Execute as células (cells) sequencialmente para reproduzir a limpeza de dados e visualizar os gráficos interativos gerados.
