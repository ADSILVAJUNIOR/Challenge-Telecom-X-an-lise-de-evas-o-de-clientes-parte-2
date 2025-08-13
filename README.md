# Challenge-Telecom-X-an-lise-de-evas-o-de-clientes-parte-2

Este projeto de Data Science foi desenvolvido para analisar dados de uma empresa de telecomunicações fictícia, a Telecom X, com o objetivo de identificar os fatores que levam à evasão de clientes (churn). O foco é encontrar padrões e variáveis que indiquem uma alta propensão de cancelamento, fornecendo insights estratégicos para a retenção.

## 🎯 Objetivo
Identificar as principais causas de churn.

Construir modelos preditivos para prever quais clientes têm maior probabilidade de cancelar seus serviços.

Gerar insights estratégicos que possam ser usados pela empresa para reduzir o churn.

## 🧰 Tecnologias e Ferramentas
Linguagem: Python 3

Bibliotecas: Pandas, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn

Ambiente: Jupyter Notebook

## 🗂️ Metodologia e Estrutura do Projeto
O projeto seguiu um fluxo de trabalho padrão em ciência de dados:

Extração e Carga: Importação de um dataset com mais de 7.000 clientes.

Tratamento de Dados:

Normalização de colunas aninhadas e conversão de colunas categóricas.

Criação de variáveis como Contas_Diarias e remoção de colunas irrelevantes.

Análise Exploratória (EDA):

Visualização da taxa de evasão e comparação entre variáveis.

Modelagem Preditiva:

Balanceamento de classes com SMOTE.

Treinamento e avaliação de modelos como DummyClassifier, DecisionTreeClassifier, RandomForestClassifier e KNN.

Relatório Final: Resumo dos padrões relevantes e sugestões de estratégias de retenção.

## 📌 Principais Insights
A análise de dados revelou os seguintes padrões:

Taxa de Churn: Cerca de 27% dos clientes cancelaram o serviço, um índice considerável.

Contrato: Clientes com contratos mensais e menos tempo de contrato evadem mais.

Pagamento: A forma de pagamento boleto por correio está fortemente associada ao churn.

Serviços Adicionais: Clientes sem serviços adicionais, como streaming ou suporte técnico, tendem a cancelar com maior frequência.

Cobrança: Cobranças mensais mais altas estão associadas à evasão.

## 📈 Desempenho dos Modelos
Modelo	Acurácia	Precisão (Classe 1)	Recall (Classe 1)	F1-Score (Classe 1)
DummyClassifier	0,7348	-	-	-
Árvore de Decisão	0,7973	0,60	0,60	0,60
Random Forest	0,8200	0,68	0,51	0,58
KNN	0,7683	0,53	0,52	0,53

Export to Sheets
O Random Forest obteve a melhor acurácia, enquanto a Árvore de Decisão apresentou um melhor equilíbrio entre precisão e recall para a classe de evasão (classe 1).

## 🚀 Como Executar o Projeto
Clone este repositório:

Bash

git clone https://github.com/elsonandrade/challenge-3-alura.git
Execute o notebook em seu ambiente Jupyter:

Bash

jupyter notebook Challenge_Telecom_X_Parte2_Elson.ipynb
O arquivo de dados (dados_tratados.csv) já deve estar incluído no repositório.
