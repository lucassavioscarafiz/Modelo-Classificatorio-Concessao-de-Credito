# Modelo-Preditivo-Concessao de Credito

## 1.0 OBJETIVO DO CASE

Neste case irei abordar a criação de **modelos preditivos supervisionados, de classificação**, utilizando os principais algoritmos de Machine Learning, e irei testar sua performance e taxa de acerto visando buscar o melhor modelo de risco preditivo criado.

Para a criação de modelos classificatórios utilizarei um dataset de risco de concessão de crédito, onde o objetivo é classificar os clientes em altas chances de concessão e baixas chances de concessão de acordo com suas informações pessoais de cunho pessoal e financeiro.


## 2.0 METODOLOGIA

Utilizei algoritmos de Machine Learning como: `Regressão Logística`, `DecisionTree`, `RandomForest`, `KNN`, `Bagging`, `GradientBoostingClassifier` e `XGBoost` para buscar o melhor modelo classificatório de acordo com o **alto risco** de concessão de crédito, além de importantes métricas de pontuação do modelo como: `Acurácia`, `Precisão`,`Recall`,`Curva ROC` e `AUC` (Area Under the roc Curve). Também foi utilizado `GridSearch` e `RandomizedSearch` para encontrar os melhores hiperparâmetros de cada modelo de forma que pudesse aperfeiçoar o modelo classificatório.

Cada modelo terá uma acurácia e uma AUC diferente do outro e o ideal não é ficar preso apenas à métricas e indicadores, e pensar no case de negócios. O objetivo é saber se devemos ou não conceder crédito à alguma pessoa, e cada banco terá um perfil, seja ele conservador ou não, então nosso modelo não pode errar muito as previsões.

Ainda que um modelo tenha uma acurácia menor que o outro, isso não significa que ele seja necessariamente pior. O objetivo é evitar ao máximo a concessão de crédito para pessoas arriscadas. É claro que o modelo não é perfeito e vai deixar de conceder crédito para pessoas que "mereciam", porém o mais importante é o modelo errar o menos possível na concessão de crédito para pessoas com **alto risco**.Se o modelo previu o cliente como 0 (Sem risco) quando na verdade ele é 1 (Arriscado), então o modelo concedeu crédito para uma pessoa arriscada, e esse é o erro crucial que o modelo deve evitar. Então esse é o principal indicador que irei visualizar, além da AUC e da Acurácia.

## 3.0 RESULTADOS

A tabela abaixo indica os valores de Acurácia, precisão e recall médio, AUC e quantas pessoas de alto risco tiveram concessão de crédito de forma errônea do modelo vencedor que foi construído utilizando o algoritmo `GradientBoostingClassifier` com os melhores hiperparâmetros encontrados pelo `GridSearch`.

Acurácia Média  | Precisão Média | Recall Média| AUC   | Erros |
--------------  | -------------- | ----------- | ----- | ----- |
76.0%           | 66.0%          | 50.0%       | 75.5% | 43    |

* Matriz de Confusão e Curva ROC do modelo vencedor

![image](https://user-images.githubusercontent.com/81670585/221262798-d58c8d95-83eb-4293-8dd4-dfa2723e0df0.png)


<h3 align="left">Contato:</h3>
<p align="left">
<a href="https://linkedin.com/in/lucassavioscarafiz" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="lucassavioscarafiz" height="30" width="40" /></a>
</p>

📫 **lucassavioscarafiz@gmail.com**

<h3 align="left">Linguagens e Ferramentas:</h3>
<p align="left"> <a href="https://cloud.google.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a> <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a> </p>
