# Titanic Survival Prediction - Machine Learning Model Battle
Sobre o projeto

Este projeto tem como objetivo prever a sobrevivência de passageiros do Titanic utilizando técnicas de Machine Learning, com foco na comparação de diferentes algoritmos de classificação.

Mais do que apenas construir um modelo preditivo, o projeto foi desenvolvido como uma batalha de modelos (Model Battle), comparando diferentes abordagens para identificar qual apresenta melhor desempenho em capacidade de generalização.

⸻

Objetivo

Desenvolver modelos preditivos para estimar a sobrevivência de passageiros com base em características demográficas e socioeconômicas, além de avaliar o impacto de técnicas de pré-processamento, balanceamento e ajuste de hiperparâmetros.

⸻

Tecnologias utilizadas
	•	Python
	•	Pandas
	•	NumPy
	•	Matplotlib
	•	Seaborn
	•	Scikit-learn
	•	XGBoost
	•	Imbalanced-learn (SMOTE)
	•	Joblib

Fluxo do projeto

1. Análise exploratória (EDA)
	•	Distribuição da variável target
	•	Análise de sobrevivência por sexo
	•	Relação entre classe social e sobrevivência
	•	Distribuição de idade
	•	Correlação entre variáveis

2. Pré-processamento
	•	Tratamento de valores ausentes
	•	Encoding de variáveis categóricas
	•	Padronização de dados

3. Feature Engineering

Criação e transformação de variáveis relevantes para melhoria da performance dos modelos.

4. Balanceamento de classes

Aplicação de SMOTE para avaliação do impacto no desempenho.

5. Modelagem

Treinamento e comparação entre:
	•	Random Forest
	•	XGBoost
	•	Support Vector Machine (SVM)

6. Hyperparameter Tuning

Otimização de hiperparâmetros para melhorar performance.

Resultados
| Modelo        | Kaggle Score
| Random Forest | 0.75119
| XGBoost       | 0.73200
| SVM           | 0.78468

Melhor modelo: Support Vector Machine(SVM)

Visualizações

Distribuição da variável alvo

(Adicionar imagem)

Sobrevivência por sexo

(Adicionar imagem)

Sobrevivência por classe

(Adicionar imagem)

Correlação entre variáveis

(Adicionar imagem)

Comparação final dos modelos

(Adicionar imagem)

⸻

Principais insights
	•	Sexo foi a variável mais determinante para sobrevivência.
	•	Passageiros de classes mais altas tiveram maior taxa de sobrevivência.
	•	Feature engineering impactou positivamente a performance.
	•	O balanceamento com SMOTE melhorou métricas de recall.
	•	O SVM apresentou melhor capacidade de generalização no Kaggle.

Autor: 
Marcos Vinícius 

