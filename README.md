# Projeto de Detecção de Fraude em Transações Financeiras
## Descrição do Projeto
Este projeto utiliza o conjunto de dados "Synthetic Financial Datasets for Fraud Detection" disponível no Kaggle, com o objetivo de simular transações financeiras legítimas e fraudulentas. O desafio principal é criar um modelo capaz de classificar corretamente essas transações com a menor taxa de erro possível, visando melhorar a experiência do cliente e reduzir prejuízos financeiros para as instituições financeiras.

O foco é a detecção de transações fraudulentas em meio a uma grande quantidade de transações legítimas, o que representa um grande desafio devido à desbalanceamento das classes e à complexidade dos dados.
## Objetivo

O objetivo deste projeto é desenvolver um modelo preditivo capaz de identificar transações fraudulentas, analisando um conjunto de dados sintético que simula transações reais. As principais metas são:

- **Detecção de fraudes**: Classificar corretamente transações fraudulentas e legítimas.
- **Minimização de erros**: Reduzir o erro de classificação, maximizando a acurácia e minimizando as taxas de falsos positivos e falsos negativos.
- **Avaliação de modelos**: Comparar e avaliar o desempenho de diferentes algoritmos de aprendizado de máquina para este problema.




## Tecnologias e Ferramentas Usadas

 **Linguagem de Programação**:
 - Python
  
 **Bibliotecas para Análise e Modelagem de Dados** 
- Pandas
- Nunpy
- MatplotLib
- Seaborn
- Scikit-learn
- Keras
  
 **Ambiente de Desenvolvimento**:
- Vscode


## Metodologia
- **Análise Exploratória de Dados (EDA)**
- **Pré-processamento**
- **Modelagem**
- **Avaliação**

## Resultados 
## Resultados

Após a Análise Exploratória de Dados (EDA) e o pré-processamento, testei cinco modelos de aprendizado de máquina para avaliar qual apresentaria o melhor desempenho na tarefa de detecção de fraudes. Os modelos testados foram:

- **RandomForestClassifier**
- **LogisticRegression**
- **KNeighborsClassifier**
- **XGBClassifier**
- **LSTM** (Long Short-Term Memory)

O modelo **RandomForestClassifier** obteve o melhor desempenho entre os modelos testados, apresentando uma boa combinação de precisão e recall, além de ser robusto em relação ao desbalanceamento de classes no conjunto de dados.

Para melhorar ainda mais o desempenho do modelo, realizei um processo de **fine-tuning** utilizando o **GridSearchCV** para otimizar os hiperparâmetros do **RandomForestClassifier**. Após o ajuste, o modelo final obteve uma **acurácia de 99,84%**, demonstrando uma excelente capacidade de identificar transações fraudulentas.

Além da acurácia, outras métricas de avaliação, como **Precision**, **Recall**, **F1-Score** e **Matriz de Confusão**  também foram analisadas para garantir que o modelo não fosse tendencioso para a classe majoritária (transações legítimas) e para otimizar a detecção das transações fraudulentas, minimizando os falsos negativos.
