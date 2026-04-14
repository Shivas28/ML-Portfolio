# 🧠 Deep Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)

> Neural network architectures for classification and sequential time-series forecasting tasks.

---

## 📚 Notebooks

# 🔊 1. Neural Networks — Sonar Mine vs Rock Classification

## 📌 Overview
Builds and tunes an ANN to classify sonar signals as either mines or rocks, with manual hyperparameter search across layer sizes, activations, and learning rates.

## 📂 Dataset
- **File:** `sonardataset.csv`
- **Target:** `Y` (M = Mine, R = Rock)
- **Features:** 60 sonar frequency features

## 🔍 What's Inside
- EDA — class distribution, correlation heatmap (first 10 features)
- LabelEncoder + StandardScaler
- Baseline ANN: `Dense(64, relu) → Dense(32, relu) → Dense(1, sigmoid)`
- Manual grid search over 18 combinations: layer sizes `[64], [128,64], [128,64,32]`, activations `relu/tanh`, learning rates `0.01/0.001/0.0001`
- Training accuracy curve over epochs
- Confusion matrix for tuned model

## 📊 Key Results
- Tuned model outperformed baseline
- Safety-critical context — Recall for mines (M) is prioritized

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn` `tensorflow` `keras`

---

# 🥛 2. RNN — Monthly Milk Production Forecasting

## 📌 Overview
Forecasts monthly milk production 12 months into the future using SimpleRNN, LSTM, and GRU models on a classic time-series dataset.

## 📂 Dataset
- **File:** `monthly_milk_production.csv`
- **Target:** `Production` (monthly milk output)

## 🔍 What's Inside
- Time-series EDA — trend plot, seasonal decomposition (period=12), ACF/PACF plots
- MinMaxScaler normalization
- Sequence creation with lookback window of 12 months
- 70/15/15 train/validation/test split
- **SimpleRNN** vs **LSTM** vs **GRU** comparison
- Evaluation — RMSE, MAE, MAPE
- 12-month future forecast with all three models plotted

## 📊 Models Compared
| Model | Metric |
|-------|--------|
| SimpleRNN | Baseline |
| LSTM | Better long-term memory |
| GRU | Faster, similar to LSTM |

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `scikit-learn` `tensorflow` `keras` `statsmodels`

---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| Artificial Neural Networks | `01_Neural_Networks.ipynb` |
| RNN / LSTM / GRU | `02_RNN.ipynb` |

---

## 🛠️ How to Run

```bash
git clone https://github.com/Shivas28/ML-Portfolio.git
cd ML-Portfolio/05_Deep_Learning
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
