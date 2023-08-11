# TitanicDisaster
Titanic Machine Learning from **[Disaster](https://www.kaggle.com/competitions/titanic/overview)**

![image](https://github.com/seppdaniel/TitanicDisaster/blob/main/img/Chart.JPG)
![image](https://github.com/seppdaniel/TitanicDisaster/assets/53501792/f37e2be2-8175-460b-b38f-d7040b8079f1)

## Step 1: Initial Model
In this step, an overview of the dataset was visualized using ydata-profiling, a library capable of generating a comprehensive dataset description.
Columns with high cardinality were eliminated, and missing values were treated using mean and mode imputation. All textual columns were removed.
Three Machine Learning models were created: Decision Tree, KNN, Logistic Regression. These models were evaluated using accuracy and confusion matrix.
- Kaggle's public score returned: 0.66746

## Step 2: Text Variable Treatment
In the second step, the primary focus was to preprocess text variables for effective integration into the proposed model.
For this treatment, lambda functions and OneHotEncoder were employed.
Three Machine Learning models were used: Decision Tree, KNN, Logistic Regression. Evaluation was based on accuracy and confusion matrix.
- Kaggle's public score returned: 0.75358

## Step 3: Business Insight Deepening and Enhanced Data Treatment
In the third step, the goal was to gain a deeper understanding of the data to facilitate enhanced treatment and potentially improve the prior results.
Accomplishments:
Enhanced comprehension of SibSp (number of siblings/spouses aboard the disaster) and Parch (number of parents/children aboard the Titanic) columns, resulting in the creation of two new columns: total family members aboard the ship and passenger's solo travel status.
Lastly, a correlation analysis of all variables was conducted to select those most relevant to the model.
Three Machine Learning models were used: Decision Tree, KNN, Logistic Regression. Evaluation was based on accuracy and confusion matrix.
- Kaggle's public score returned: 0.77033

## Step 4: Exploring Additional Prediction Algorithms
In this step, all columns were retained, and new algorithms were introduced for model monitoring and validation.
The algorithms utilized in this stage include Logistic Regression (retained due to its superior performance in earlier steps), RandomForest, and MLPClassifier (Neural Networks).
MLPClassifier (a Neural Network algorithm) exhibited the highest validation accuracy among all previously seen models. However, upon testing this model on the submission dataset, its performance deteriorated compared to Step 3, suggesting potential overfitting in the model.
- Kaggle's public score returned: 0.69856

## Step 5: GridSearchCV Utilization and Optimal Parameter Determination
The GridSearchCV technique is now employed to identify optimal parameters for the three models utilized in the previous step.
In this instance, the chosen model was 'RandomForest,' which exhibited substantial improvements over Step 4 and surpassed its performance.
- Kaggle's public score returned: 0.78229

__________
Portuguese
__________

## [Etapa 1: Primeiro Modelo](https://github.com/seppdaniel/TitanicDisaster/blob/main/titanic_pt1.ipynb)
- Nesta etapa foi visualizado um resumo da base utilizando o ydata-profiling, biblioteca capaz de gerar toda a descrição do dataset
  - Eliminação de colunas com **elevada cardinalidade**, tratamento de **valores vazios** utilizando média e a moda das variáveis e todas as **colunas de texto** foram eliminadas
  - Houve a criação de 3 modelos de Machine Learning: **Árvore de Classificação, KNN, Refressão Logística** e avaliamos esses modelos utilizando a acurácia e a matriz de confusão
- **O score público retornado pelo Kaggle foi: 0.66746**
 
## [Etapa 2: Tratamento das variáveis de texto](https://github.com/seppdaniel/TitanicDisaster/blob/main/titanic_pt2.ipynb)
- Na segunda etapa, o foco principal foi tratar as variáveis de texto para conseguirmos utilizar todas as variáveis no modelo proposto
  - Para fazer este tratamento, foi utilizado **lambda function** e **OneHotCoder**
  - Foram utilizados 3 modelos de Machine Learning: **Árvore de Classificação, KNN, Refressão Logística** e avaliamos esses modelos utilizando a acurácia e a matriz de confusão
- **O score público retornado pelo Kaggle foi: 0.75358**

## [Etapa 3: Aprofundamento no negócio e melhorando os tratamento dos dados](https://github.com/seppdaniel/TitanicDisaster/blob/main/titanic_pt3.ipynb)
- Na terceira etapa, o objetivo era **entender melhor os dados** para **fazer um melhor tratamento** e tentar melhorar o resultado obtido anteriormente.
- O que foi feito:
  - Melhor entendimento das colunas **SibSp** (nº de irmãos/cônjuges a bordo do desastre) e **Parch** (nº de pais/filhos a bordo do Titanic) e foram **criadas 2 novas colunas: total de familiares a bordo do nabio e se o passageiro estava sozinho ou não**
  - Por fim, foi analisada a **correlação de todas as variáveis** para selecionar aquelas que mais faziam sentido para o modelo
  - Foram utilizados 3 modelos de Machine Learning: **Árvore de Classificação, KNN, Refressão Logística** e avaliamos esses modelos utilizando a acurácia e a matriz de confusão
- **O score público retornado pelo Kaggle foi: 0.77033**

## [Etapa 4: Selecionando outros algoritmos para fazer a previsão](https://github.com/seppdaniel/TitanicDisaster/blob/main/titanic_pt4.ipynb)
- Nesta etapa todas as colunas serão mantidas, e utilizaremos novos algoritmos para o monitoramento e a verficação do modelo
- Os algoritmos que vamos utilizar nessa etapa são a **Regressão Logística** (será mantido, pois foi o modelo que apresentou melhores resultados nas etapas anteriores, **RandomForest e MLPClassifier (Redes Neurais)
- O MLPClassifier (um algoritmo de Redes Neurais) obteve a maior acurácia nos dados de validação entre todos os modelos vistos até agora, porém ao usar esse modelo nos dados de teste (tabela de submissão na competição) o resultado foi pior do que na etapa 3, mostrando que **provavelmente tivemos um overfitting no nosso modelo**
- O **score público retornado pelo Kaggle foi: 0.69856

## [Etapa 5: Utilizando o GridSearchCV e determinando os melhores parâmetros](https://github.com/seppdaniel/TitanicDisaster/blob/main/titanic_pt5.ipynb)
- Agora o GridSearchCV foi utilizado para determinar os melhores parâmetros para os três modelos que foram utilizados na etapa anterior.
- Neste caso, o modelo escolhido foi 'RandomForest' que apresentou melhorias consideráveis em relação a etapa 4 e foi melhor que na etapa 4.
- O **score público retornado pelo Kaggle foi: 0.78229
