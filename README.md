# 🕵️‍♂️ Detecção de Anomalias em Transações

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Este projeto aplica **Machine Learning** para detectar possíveis fraudes em transações financeiras.  
O objetivo é construir um modelo capaz de identificar padrões anômalos em dados altamente desbalanceados, utilizando técnicas de classificação e interpretabilidade.

---

## 🚀 Tecnologias utilizadas
- **Python 3.10**
- **[XGBoost](ca://s?q=O_que_e_XGBoost)** para classificação
- **[Scikit-learn](ca://s?q=O_que_e_scikit_learn)** para métricas e pré-processamento
- **[SHAP](ca://s?q=O_que_e_SHAP)** para interpretabilidade
- **Pandas / NumPy** para manipulação de dados
- **Matplotlib / Seaborn** para visualização

---

## 📂 Estrutura do projeto
- `deteccao_de_anomalias_em_transacoes.ipynb` → Notebook principal com todo o pipeline:
  - Carregamento e exploração dos dados
  - Treinamento do modelo
  - Avaliação com métricas (precision, recall, f1-score, AUC)
  - Explicabilidade com gráficos SHAP

---

## 📊 Resultados
O modelo treinado obteve:
- **AUC ≈ 0.95**
- **Recall ≈ 0.82** para a classe de fraude
- Excelente desempenho na classe majoritária, com **accuracy ≈ 1.00**

### Importância das variáveis (SHAP)
O SHAP foi utilizado para interpretar o modelo e identificar quais variáveis mais influenciam na detecção de fraude:

![Exemplo de gráfico SHAP](docs/shap_bar_example.png)

---

## ⚙️ Como executar
1. Clone o repositório:
```bash
  git clone https://github.com/cleitonrs/deteccao-de-anomalias-em-transacoes.git
  cd deteccao-de-anomalias-em-transacoes
```
2. Instale as dependências:
  ```bash
  pip install -r requirements.txt
```
3. Abra o Jupyter Notebook:
  ```bash
  jupyter notebook deteccao_de_anomalias_em_transacoes.ipynb
```
