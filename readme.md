
# 1. Competição da Alura de Fraudes em Transações de Cartão de Crédito - Kaggle (04/2024)

## 1.1 **🏆🏆 VENCEDOR DA COMPETIÇÃO 🏆🏆**

<br>

<img src="./Images/Kaggle Leaderboard.PNG" width="100%">

## 1.2 Link para a Competição:
[Competição Kaggle](https://www.kaggle.com/competitions/fraude-em-transaes-de-carto-de-crdito/overview)

# 2. Descrição

O objetivo da competição era prever a probabilidade de uma transação de cartão de crédito ser fraude ou não. A competição durou cerca de 3 meses, de 30 de Janeiro de 2024 a 5 de Abril de 2024. Um dataset foi disponibilizado para treinamento dos modelos de Machine Learning, enquanto outro foi utilizado para avaliar o resultado final.

## 2.1 Contexto
Em 2022, o volume de transações com cartões de crédito cresceu cerca de 35%, segundo a ABECS, atingindo R$ 3,31 trilhões e movimentando a maioria (52,9%) de todo o consumo das famílias brasileiras no período. Isso mostra a relevância de detectar fraudes nas transações de cartão de crédito.

## 2.2 Jupyter Notebook
O projeto foi realizado usando o Google Colab. Você pode acessá-lo clicando no botão abaixo:

<a href="./Kaggle_Competition_Award.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

## 2.3 Bibliotecas Utilizadas
Este projeto utiliza as seguintes bibliotecas:

- `Pandas`
- `Numpy`
- `Plotly`
- `Sklearn`

## 2.4 Pré-processamento de Dados
Para a utilização de técnicas de Machine Learning, é importante realizar o pré-processamento dos dados de maneira adequada. Foram utilizadas as seguintes técnicas:

- **OneHotEncoder**
- **make_column_transformer**
- **StandardScaler**
- **SMOTE** (para lidar com classes desbalanceadas)

## 2.5 Modelos Utilizados
Os seguintes modelos de machine learning foram aplicados para a classificação:

- `DummyClassifier`
- `DecisionTreeClassifier`
- `RandomForestClassifier`
- `XGBClassifier`
  
O modelo que apresentou melhor acurácia foi o `RandomForestClassifier`, com uma **acurácia de 99,8794% e uma precisão de 99,885%!**

| Rank | Model                    | Accuracy  | Precision |
|------|--------------------------|-----------|-----------|
| 1    | RandomForest             | 0.9987  | 0.9988  |
| 2    | DecisionTreeClassifier    | 0.9974  | 0.9974  |
| 3    | XGBClassifier            | 0.9625  | 0.9831  |
| 4    | DummyClassifier          | 0.5000  | 0.2499  |

## 2.6 Comentários Gerais
Participar da competição foi uma oportunidade valiosa de aprendizado, onde o foco principal foi no desenvolvimento de um modelo funcional, considerando o tempo reduzido. Com o término, dediquei tempo a aprimorar técnicas e revisar o trabalho com mais calma, o que me levou às sugestões de melhorias descritas abaixo.

# 3. Melhorias / Próximos Passos
Com base na experiência adquirida durante a competição, identifiquei diversas áreas para aprimoramento que podem contribuir para o desenvolvimento de modelos de machine learning mais robustos e eficientes.

## 3.1 Análise e Visualização dos Dados 
É possível aprimorar a visualização dos dados, criando gráficos mais informativos que destacam padrões e outliers. Isso ajuda a entender a distribuição dos dados e as relações entre variáveis, facilitando insights mais profundos. Um exemplo é a aplicação do módulo `ydata-profiling` e da biblioteca `ProfileReport`. Além disso, bibliotecas como `matplotlib` e `seaborn` podem ser utilizadas para criar visualizações personalizadas que atendam a necessidades específicas.

## 3.2 Validação Cruzada
Implementar validação cruzada garante que o modelo seja avaliado de forma robusta. Isso evita o overfitting, ao testar o desempenho do modelo em diferentes subconjuntos dos dados e assegurando uma avaliação mais realista. Uma abordagem como `StratifiedKFold` pode ser utilizada para garantir a representação adequada das classes.

## 3.3 Hiperparâmetros
O ajuste fino de hiperparâmetros pode melhorar significativamente a performance do modelo. Automatizar o processo de busca pelos melhores valores usando técnicas como `GridSearch`, `RandomizedSearch` ou até mesmo `Bayesian Optimization` pode levar a resultados mais otimizados.

## 3.4 Pipeline
A criação de um pipeline de machine learning automatiza o processo de transformação de dados e modelagem, garantindo reprodutibilidade e escalabilidade, facilitando também a manutenção ao longo do tempo. O uso do `Pipeline` do `sklearn` pode ser um exemplo prático dessa implementação.

## 3.5 Redução de Dimensionalidade
A aplicação de técnicas como PCA pode reduzir o número de features no conjunto de dados, simplificando o modelo e melhorando o desempenho, especialmente em datasets com muitas variáveis correlacionadas. Alternativas como t-SNE ou UMAP também podem ser consideradas para visualizações mais eficazes.

## 3.6 Seleção de Atributos
Implementar técnicas de seleção de atributos, como `SelectKBest` ou `Recursive Feature Elimination`, permite identificar as variáveis mais relevantes, reduzindo a complexidade do modelo e aumentando a interpretabilidade sem perda significativa de precisão. Além disso, técnicas baseadas em modelos, como Lasso, podem ser utilizadas para seleção e regularização.

# 4. Conecte-se Comigo:
<a href="https://www.linkedin.com/in/felipe-dick" target="_blank">
    <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="Link" width="30" height="30">    
</a>
<br>
<br>

