
# 1. Competição da Alura de Fraudes em Transações de Cartão de Crédito - Kaggle (04/2024)

## 1.1 **🏆🏆 VENCEDOR DA COMPETIÇÃO 🏆🏆**
O modelo final obteve um score de 99,897%, conquistando o **primeiro lugar** na competição.

![Leaderboard da Competição](./Images/Kaggle%20Leaderboard.PNG)

## 1.2 Link para a Competição:
[Competição Kaggle](https://www.kaggle.com/competitions/fraude-em-transaes-de-carto-de-crdito/overview)

## 1.3 Descrição

O objetivo da competição foi prever a probabilidade de uma transação de cartão de crédito ser fraudulenta ou não. A competição durou de 30 de janeiro a 5 de abril de 2024, e os participantes receberam datasets para treinar e avaliar seus modelos de Machine Learning.

## 1.4 Contexto
Em 2022, o volume de transações com cartões de crédito cresceu cerca de 35%, segundo a ABECS, atingindo R$ 3,31 trilhões e movimentando a maioria (52,9%) do consumo das famílias brasileiras. Isso ressalta a importância de detectar fraudes em transações de cartão de crédito.

---

# 2. O Projeto

## 2.1 Jupyter Notebook / Google Colab
O projeto foi realizado usando o Google Colab. Você pode acessá-lo abaixo

[Abrir](https://github.com/felipedick/1st-place-Machine-Learning-Competittion/blob/main/Alura_Fraud_Transaction_Competition_Award.ipynb)

## 2.2 Bibliotecas Utilizadas
Este projeto utilizou as seguintes bibliotecas:

- `Pandas`
- `Numpy`
- `Plotly`
- `Sklearn`

## 2.3 Coleta dos Dados
Os dados foram disponibilizados através da plataforma Kaggle ([link dos dados](https://www.kaggle.com/competitions/fraude-em-transaes-de-carto-de-crdito/data)).

Arquivos coletados:
- **treino.csv.xz** - Arquivo de treino
- **teste.csv.xz** - Arquivo de teste
- **exemplo_submissao.csv** - Exemplo do formato de submissão

Foi realizada uma análise inicial usando `.info()` para entender as variáveis disponíveis.

## 2.4 Limpeza dos Dados
A etapa de limpeza dos dados incluiu a remoção de colunas irrelevantes ou com muitos valores ausentes. As seguintes variáveis foram removidas:

- **merch_lat**, **merch_long**, e **zip**: Alto número de valores ausentes (10% do total).
- **ssn**, **cc_num**, **first**, **last**, **street**, **acct_num**, **trans_num**, e **dob**: Dados específicos que poderiam causar overfitting.
- **trans_date** e **trans_time**: Utilizou-se o campo **unix_time** para representar o tempo.
- **city** e **state**: Substituídos pela variável **population**.
- **merchan**, **lat** e **long**: Considerados pouco relevantes.

Após a remoção de colunas, tratamos os valores ausentes.

## 2.5 Análise Exploratória dos Dados (EDA)
A EDA teve como foco a derivação de novas variáveis e a validação de hipóteses de negócio, além de investigar padrões e anomalias nos dados. Dada a limitação de tempo, a EDA foi limitada às seguintes análises:

- **Distribuição da variável alvo por gênero**: Identificado o desbalanceamento de classes (fraude vs não fraude).
- **Boxplot do valor das transações**: Investigamos a hipótese de que transações acima de determinado valor seriam fraudes. A hipótese foi rejeitada, já que transações fraudulentas variaram até $1264,23, mas houve várias transações não fraudulentas acima desse valor.

## 2.6 Modelagem dos Dados
Nesta etapa, preparamos os dados para o treinamento dos modelos, aplicando técnicas como:

- **OneHotEncoder** para variáveis categóricas.
- **StandardScaler** para normalização.
- **SMOTE** para lidar com o desbalanceamento de classes.

## 2.7 Aplicação de Algoritmos de Machine Learning
Os seguintes modelos de Machine Learning foram aplicados:

- `DummyClassifier`
- `DecisionTreeClassifier`
- `RandomForestClassifier`
- `XGBClassifier`

O **RandomForestClassifier** obteve o melhor desempenho, com uma **acurácia de 99,87%** e **precisão de 99,88%**.

| Rank | Modelo                    | Acurácia  | Precisão |
|------|---------------------------|-----------|----------|
| 1    | RandomForest               | 0.9987    | 0.9988   |
| 2    | DecisionTreeClassifier     | 0.9974    | 0.9974   |
| 3    | XGBClassifier              | 0.9625    | 0.9831   |
| 4    | DummyClassifier            | 0.5000    | 0.2499   |

## 2.8 Aplicação no Dataset de Teste
O modelo **RandomForestClassifier** foi aplicado no dataset de teste, utilizando o mesmo pré-processamento. O arquivo final obteve um score de 99,897%, garantindo o primeiro lugar na competição.

---

# 3. Comentários Gerais
Participar dessa competição foi uma excelente oportunidade de aprendizado. O foco principal foi o desenvolvimento de um modelo funcional dentro de um prazo curto. Após a competição, continuei aprimorando técnicas e revisando o projeto para identificar áreas de melhoria.

---

# 4. Melhorias / Próximos Passos

## 4.1 Análise e Visualização dos Dados
Aprimorei a visualização dos dados utilizando bibliotecas como `ydata-profiling`, `matplotlib` e `seaborn`. Esses gráficos ajudam a identificar padrões e outliers de forma mais clara.

## 4.2 Validação Cruzada
Implementar **validação cruzada** como o `StratifiedKFold` garantiria uma avaliação mais robusta do modelo, evitando overfitting.

## 4.3 Tunagem de Hiperparâmetros
O ajuste fino de hiperparâmetros, com técnicas como **GridSearch** e **RandomizedSearch**, pode melhorar ainda mais a performance do modelo.

## 4.4 Pipeline
Criar um **pipeline de machine learning** com o `Pipeline` do `sklearn` automatizaria o processo de transformação de dados e modelagem, garantindo reprodutibilidade e escalabilidade.

## 4.5 Redução de Dimensionalidade
Técnicas como **PCA** podem reduzir o número de features, simplificando o modelo e melhorando seu desempenho.

## 4.6 Seleção de Atributos
Utilizar **feature selection** com base em importância de variáveis pode reduzir a complexidade do modelo sem perder precisão.


# 5. Conecte-se Comigo:
<a href="https://www.linkedin.com/in/felipe-dick" target="_blank">
    <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="Link" width="30" height="30">    
</a>
<br>
<br>

