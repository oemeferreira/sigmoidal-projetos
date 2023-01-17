[![author](https://img.shields.io/badge/author-oemeferreira-red.svg)](https://www.linkedin.com/in/oemeferreira/) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-365/) [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/oemeferreira/portfolio/issues)

<p align="center">
  <img src="https://otripulante.com/assets/images/blog/CG_como-funciona-o-seguro-de-vida-ij_235111542.jpg" alt="Seguro de Vida"height=400px >
</p>

## **Previsão de valor de um seguro de vida**

O seguro de vida é um dos produtos mais importantes e populares no mercado de seguros, pois garante a proteção financeira da família do segurado em caso de morte. A previsão do custo de seguro de vida é um problema crítico para as empresas de seguros, pois é a base para a fixação do prêmio e, portanto, para o sucesso da empresa.

Neste projeto, utilizamos técnicas de Aprendizado de Máquina (Machine Learning) para desenvolver um modelo de regressão para prever o custo do seguro de vida. Utilizamos o conjunto de dados disponível no Kaggle, que contém informações demográficas e de saúde dos segurados, como idade, sexo, Índice de Massa Corporal (IMC), tabagismo e região.

Iniciamos o projeto com a etapa de coleta de dados, onde baixamos o conjunto de dados e o carregamos em nosso ambiente de trabalho. Em seguida, realizamos uma análise exploratória dos dados, onde verificamos a existência de valores nulos, a quantidade de valores únicos por variável e as estatísticas básicas do conjunto de dados. Além disso, plotamos uma matriz de correlação para identificar as relações entre as variáveis e verificamos se existem outliers presentes nos dados.

Na etapa seguinte, preparamos os dados para o treinamento do modelo. Utilizamos o framework PyCaret para automatizar o processo de seleção e otimização de modelos. O PyCaret aplica o OneHotEncoder automaticamente em todos os valores considerados categóricos, portanto não precisamos transformar os dados manualmente. Também passamos o parâmetro normalize = True para que o PyCaret faça a padronização dos dados automaticamente.

Utilizamos o R² como métrica para escolher o melhor modelo, e verificamos que o melhor modelo para nosso cenário é o GBR (Gradient Boost Regressor). Realizamos algumas previsões com esse modelo e comparamos com os dados reais, e o modelo se mostrou eficiente.

Por fim, é importante destacar que, apesar de utilizarmos técnicas de Auto Machine Learning, é fundamental entender o problema e os dados antes de selecionar qualquer modelo ou técnica. Além disso, existem diversas melhorias que podem ser feitas nesse projeto, como avaliar outros modelos e/ou outras métricas de desempenho, ou realizar outros tratamentos nos dados.

Confira o notebook da [Previsão de valor de um seguro de vida](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/AutoML-Regressao/Previsao_custo_seguro_vida_com_PyCaret.ipynb)

**Links para me acharem:**
* [LinkedIn](https://www.linkedin.com/in/oemeferreira)
* [Medium](https://medium.com/@emeferreira)
