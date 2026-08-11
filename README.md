# Projetos de Ciência de Dados

Seis projetos de análise e machine learning sobre dados públicos, cada um partindo de uma pergunta de negócio e terminando em um resultado mensurável.

Desenvolvidos durante o curso **Data Science na Prática**, da Sigmoidal.

---

## Projetos

### 1. [Análise de Dados do Airbnb de Lisboa](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/Analise-de-Dados-Pandas/Analisando_os_Dados_do_Airbnb.ipynb)

Análise exploratória dos anúncios de Lisboa: distribuição de preços, tipos de imóvel, concentração por bairro e identificação de outliers que distorcem a média.

`Pandas` · `Matplotlib` · `Seaborn`

---

### 2. [Panorama do COVID-19 no Brasil](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/VIsualizacao%20de%20Dados/Panorama_do_COVID_19_no_Brasil.ipynb)

Análise da evolução da pandemia no Brasil a partir dos dados públicos do *Our World in Data*, com foco em séries temporais de casos, óbitos e vacinação.

`Pandas` · `NumPy` · `Matplotlib` · `Seaborn`

---

### 3. [Detecção de Fraude em Cartões de Crédito](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/Introducao-Machine-Learning/Deteccao_de_Fraude_em_Cartoes_de_Credito.ipynb)

Classificação de transações fraudulentas em uma base fortemente desbalanceada — o desafio central do problema, já que acurácia alta é trivial quando fraude é uma fração mínima dos casos.

`Scikit-learn` · `Imbalanced-learn` · `Scikit-plot` · `Pandas`

---

### 4. [Churn Prediction para empresa de telecomunicações](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/Machine-Learning-Avancado/Churn_Prediction_para_empresa_Hyperconnect_Telecom.ipynb)

Previsão de cancelamento de planos. A métrica escolhida foi **recall**, e não acurácia: deixar de identificar um cliente que vai cancelar custa mais que abordar um cliente que ficaria.

> **Resultado:** Logistic Regression com **recall de 87%** na validação cruzada e **87% no conjunto de teste** — a proximidade entre os dois indica que o modelo generalizou.

`Scikit-learn` · `XGBoost` · `LightGBM` · `Imbalanced-learn`

---

### 5. [Previsão de custo de Seguro de Vida](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/AutoML-Regressao/Previsao_custo_seguro_vida_com_PyCaret.ipynb)

Regressão para estimar o valor de apólices, usando AutoML para comparar e otimizar modelos automaticamente.

> **Observação do projeto:** AutoML acelera a seleção de modelos, mas não substitui o entendimento prévio do problema e dos dados — usá-lo como atalho para pular a etapa de análise leva a resultados que ninguém sabe defender.

`PyCaret` · `Pandas` · `Seaborn`

---

### 6. [Classificação de risco gestacional](https://github.com/oemeferreira/sigmoidal-projetos/blob/main/AutoML-Classificacao/Classifica%C3%A7%C3%A3o_de_risco_gestacional_com_PyCaret.ipynb)

Classificação de saúde fetal a partir de exames de cardiotocografia, com o objetivo de apoiar a prevenção da mortalidade infantil e materna.

> **Resultado:** **LightGBM** selecionado como melhor modelo pela comparação automática do PyCaret.

`PyCaret` · `SweetViz` · `Pandas`

---

## Como rodar

Os projetos usam dois ambientes diferentes, porque o PyCaret fixa `matplotlib<3.8.0` e conflita com as versões usadas nos demais notebooks.

**Projetos 1 a 4**

```bash
pip install -r requirements.txt
jupyter notebook
```

**Projetos 5 e 6, que usam PyCaret**

```bash
python -m venv .venv-pycaret
source .venv-pycaret/bin/activate     # Windows: .venv-pycaret\Scripts\activate
pip install -r requirements-pycaret.txt
jupyter notebook
```

---

## Estrutura

```
Analise-de-Dados-Pandas/       Airbnb Lisboa
VIsualizacao de Dados/         COVID-19 no Brasil
Introducao-Machine-Learning/   Deteccao de fraude
Machine-Learning-Avancado/     Churn prediction
AutoML-Regressao/              Seguro de vida
AutoML-Classificacao/          Risco gestacional
data/                          bases utilizadas
```

Cada pasta tem seu próprio README com o detalhamento do projeto.

---

## Contato

[LinkedIn](https://www.linkedin.com/in/oemeferreira) · [Medium](https://medium.com/@emeferreira)

---

## Observações

Todos os dados são públicos e de uso educacional. Nenhum resultado aqui representa operação real de empresa, e o projeto de risco gestacional não constitui ferramenta clínica.
