# Titanic Survival Prediction

### Uma batalha de modelos para previsão de sobrevivência

## Contexto do Problema

O naufrágio do Titanic é um dos desastres marítimos mais conhecidos da história e se tornou um problema clássico de Machine Learning. A competição do Kaggle propõe prever quais passageiros sobreviveram com base em características demográficas e socioeconômicas.

Este projeto busca responder à seguinte pergunta:

**Quais fatores tiveram maior influência na sobrevivência dos passageiros e qual modelo apresenta melhor desempenho preditivo?**

___

## Objetivo

Utilizar técnicas de análise de dados e Machine Learning para prever a sobrevivência dos passageiros, comparando diferentes algoritmos de classificação e avaliando o impacto de técnicas de balanceamento e ajuste de hiperparâmetros.

___

## Fonte de Dados

Os dados utilizados foram disponibilizados pela competição oficial do Kaggle:

Titanic - Machine Learning from Disaster

## Variáveis selecionadas:
-	PassengerId
-	Pclass
-	Sex
-	Age
- 	SibSp
-  Parch
-  Fare
-  Embarked

## Variável target:
- 	Survived
-	0 = Não sobreviveu
- 	1 = Sobreviveu

___

## Coleta e Tratamento de Dados

O processo de preparação incluiu:
-	Análise de valores ausentes
-	Tratamento de variáveis nulas (Age, Embarked, Fare)
-	Conversão de variáveis categóricas em numéricas
-	Padronização de variáveis para modelos sensíveis à escala
-	Separação entre variáveis independentes (X) e variável target (y)

Essas etapas foram fundamentais para garantir melhor qualidade e consistência dos dados para modelagem.

___

## Análise Exploratória de Dados (EDA)

A análise exploratória revelou padrões importantes:

Principais achados:
-	Mulheres apresentaram taxa de sobrevivência significativamente maior.
-	Passageiros da primeira classe tiveram maior probabilidade de sobreviver.
-	Passageiros mais jovens apresentaram maior taxa de sobrevivência em alguns grupos.
-	A classe social e a tarifa paga mostraram forte relação com sobrevivência.

Esses padrões indicam que fatores sociais e demográficos tiveram impacto relevante no desfecho.

___

## Feature Engineering

Foram realizadas transformações para melhorar a performance dos modelos:
-	Encoding da variável Sex
-	Encoding da variável Embarked
-	Normalização de variáveis numéricas
-	Ajustes estruturais para treinamento

Além disso, foram realizados experimentos com balanceamento utilizando SMOTE.

___

## Modelagem

Foram treinados e comparados três modelos de classificação:
-	Random Forest
-	XGBoost
-	Support Vector Machine (SVM)

## Etapas da modelagem:
-	Train/Test Split
-	Treinamento inicial (baseline)
- 	Testes com SMOTE
- Ajuste de hiperparâmetros
-	Avaliação com métricas de classificação
-	Submissão no Kaggle
  
___

## Resultados

### Comparação dos modelos
| Modelo | Kaggle Score
|___ |___:
| Randon Forest | 0.75119
| XGBoost | 0.73200
| SVM | 0.78468

**O SVM apresentou o melhor desempenho final**, superando modelos ensemble como Random Forest e XGBoost.

Esse resultado demonstra que, para este conjunto de dados, um modelo com maior capacidade de separação de fronteira apresentou melhor generalização.

___

## Visualizações

## Distribuição da variável target

![![Distribuição](figuras/)

---

### Sobrevivência por sexo

![Sobrevivencia](figuras/)

---

### Distribuição por idade

![Distribuicao](figuras/)

---
### Comparação final

![Comparacao](figuras/)

___

## Conclusões

Os resultados mostraram que fatores demográficos e socioeconômicos tiveram forte relação com a sobrevivência no Titanic.

## As variáveis mais relevantes foram:
- 	Sexo
-	Classe social
-	Idade
-	Tarifa paga

Apesar do bom desempenho dos modelos ensemble, o SVM apresentou a melhor capacidade preditiva no conjunto de teste final.

Este projeto demonstra a importância da experimentação, comparação entre modelos e técnicas de pré-processamento para construção de modelos mais robustos.

___

## Tecnologias Utilizadas
-	Python
-	Pandas
-	NumPy
-	Matplotlib
-	Seaborn
-	Scikit-learn
-	XGBoost
-	Imbalanced-learn (SMOTE)
-	Joblib
-	Kaggle

