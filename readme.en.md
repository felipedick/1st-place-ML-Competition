# Alura Kaggle competitition for fraud transaction in April/24

## **🏆🏆 AWARD 1ST PLACE 🏆🏆**
## **🏆🏆 VENCEDOR DA COMPETIÇÃO 🏆🏆**


<br>

<img src="./Images/Kaggle Leaderboard.PNG" width="100%">


## Link to Competition / Link para competição:
[https://www.kaggle.com/competitions/fraude-em-transaes-de-carto-de-crdito/code](https://www.kaggle.com/competitions/fraude-em-transaes-de-carto-de-crdito/overview)

## Description / Descriçãoo:
The goal of the competition is to predict whether a credit card transaction is fraudulent or not. The competition lasted for three months, from January 30, 2024, to April 5, 2024.

O objetivo da competição era prever qual a probablidade de uma transação de cartão de crédito ser fraude ou não. A competição durou cerca de 3 meses, de 30 de Janeiro de 2024 a 5 de Abril de 2024. Foi disponibilizado um dataset para treinamento dos modelos de Machine Learning e um dataset com amostras que foram utilizadas para avaliar o resultado final.

### Contexto
Em 2022, o volume de transações com cartões de crédito cresceu cerca de 35%, segundo a ABECS, atingindo  R$ 3,31 trilhões e movimentando a maioria (52,9%)de todo o consumo das famílias brasileiras no período. (Associação Brasileira das Empresas de Cartões de Crédito e Serviços).

## Jupyter Notebook
The project was designed using Google Colab.

O Projeto foi feito usando o Google Colab.

<a href="./Kaggle_Competition_Award.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

### Bibliotecas utilizadas
This project used the following library:

Este projeto utiliza as seguintes bibliotecas

- `Pandas`
- `Numpy`
- `Plotly`
- `Sklearn`

### Pré-processamento de Dados
Os dados foram pré-processados utilizando as seguintes técnicas:

- **OneHotEncoder**
- **make_column_transformer**
- **StandardScaler**
- **SMOTE** (para lidar com classes desbalanceadas)

### Modelos Utilizados
Os seguintes modelos de machine learning foram aplicados para a classificação:

- `DummyClassifier`
- `DecisionTreeClassifier`
- `RandomForestClassifier`
- `XGBClassifier`
  
O modelo que apresentou melhor acurácia foi o RandomForestClassifier com uma **acurácia de 99,8794% e uma precisão de 99,885%!**

| Rank | Model                    | Accuracy  | Precision |
|------|--------------------------|-----------|-----------|
| 1    | RandomForest             | 0.9987  | 0.9988  |
| 2    | DecisionTreeClassifier    | 0.9974  | 0.9974  |
| 3    | XGBClassifier            | 0.9625  | 0.9831  |
| 4    | DummyClassifier          | 0.5000  | 0.2499  |


## Connect with author:

<a href="https://www.linkedin.com/in/felipe-dick" target="_blank">
    <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="Link" width="30" height="30">    
</a>
<br>
<br>
