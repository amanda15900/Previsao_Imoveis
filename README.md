## 🏡 Projeto Individual PI1: Previsão de Preço de Imóveis (Regressão)

---

### 🎯 Objetivo

Este projeto individual (PI1) aplica técnicas de **Aprendizado de Máquina Supervisionado** para resolver um problema de **Regressão**. O objetivo principal é **prever o preço mediano de casas** (`MedHouseVal`) no estado da Califórnia, utilizando características demográficas e geográficas fornecidas pelo *California Housing Dataset*.

O projeto foca na **comparação** de desempenho entre dois modelos distintos para identificar qual se adapta melhor à complexidade do mercado imobiliário.

---

### 🤖 Modelos e Metodologia

Foram implementados e avaliados dois algoritmos de Regressão:

1.  **Regressão Linear (`LinearRegression`):** Utilizado como modelo *baseline* (linha de base) para medir a performance quando a relação entre variáveis é assumida como estritamente linear.
2.  **Random Forest Regressor (`RandomForestRegressor`):** Utilizado como um modelo mais robusto e não-linear, capaz de capturar interações complexas entre as características dos dados.

#### 📊 Métricas de Avaliação
O desempenho dos modelos foi avaliado usando o **Erro Quadrático Médio (MSE)** e o **Coeficiente de Determinação ($R^2$)**.

---

### 🔍 Estrutura do Projeto e Análise

O projeto segue as seguintes etapas obrigatórias:

1.  **ETL (Extract, Transform, Load):** Carregamento do *California Housing Dataset* (`sklearn.datasets`), verificação de valores ausentes (limpeza de dados) e divisão em conjuntos de treino e teste.
2.  **Visualização:** Utilização de `matplotlib` e `seaborn` para analisar a distribuição do preço e a correlação entre as variáveis (especialmente **`MedInc` - Renda Mediana**).
3.  **Modelagem e Treinamento:** Implementação, treinamento e previsão utilizando os dois modelos.
4.  **Análise e Interpretação:** Comparação direta dos resultados dos modelos. O **Random Forest** demonstrou superioridade significativa (obtendo um $R^2$ mais alto), indicando que a relação entre as características do imóvel e o preço é **não-linear**.

| Modelo | MSE | R² |
| :--- | :--- | :--- |
| **Regressão Linear** | $\approx 0.53$ | $\approx 0.61$ |
| **Random Forest** | $\approx 0.25$ | $\approx 0.81$ |

---

### 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Bibliotecas:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
* **Google Colab / Jupyter Notebook** 
