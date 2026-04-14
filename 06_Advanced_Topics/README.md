# 🚀 Advanced Topics

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3776AB?style=for-the-badge&logo=python&logoColor=white)

> Specialized ML applications — recommendation systems, time series forecasting, and natural language processing.

---

## 📚 Notebooks

# 🎌 1. Recommendation System — Anime Content-Based Filtering

## 📌 Overview
Builds a content-based recommendation engine for anime using cosine similarity across genre, rating, type, members and episodes.

## 📂 Dataset
- **File:** `anime.csv`
- **Features:** genre, rating, members, episodes, type

## 🔍 What's Inside
- EDA — rating distribution, type counts, boxplot
- Genre multi-label encoding using `MultiLabelBinarizer`
- OneHotEncoding on `type`, StandardScaler on numerical features
- Cosine similarity matrix computed across all anime
- `recommend(title, n, threshold)` function with adjustable similarity threshold
- Threshold analysis — 0.7 to 0.95 tested on `Steins;Gate`

## 📊 Key Insight
> Higher threshold = fewer but more relevant results. Lower threshold = broader but noisier recommendations.

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn`

---

# 💱 2. Time Series — Exchange Rate Forecasting

## 📌 Overview
Forecasts USD to AUD exchange rates using ARIMA and Exponential Smoothing, with stationarity testing and model evaluation.

## 📂 Dataset
- **File:** `exchange_rate.csv`
- **Target:** `Ex_rate` (USD to AUD daily rate)

## 🔍 What's Inside
- Time-series plot, seasonal decomposition (period=365)
- ADF test for stationarity → differencing applied (d=1 confirmed)
- ACF + PACF plots → ARIMA(1,1,1) selected
- **ARIMA(1,1,1)** model training and residual analysis
- **Exponential Smoothing** (additive trend) model
- Side-by-side forecast comparison — MAE, RMSE, MAPE

## 📊 Models Compared
| Model | MAE | RMSE | MAPE |
|-------|-----|------|------|
| ARIMA(1,1,1) | Computed | Computed | Computed |
| Exponential Smoothing | Computed | Computed | Computed |

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `scikit-learn` `statsmodels`

---

# 💬 3. NLP — Amazon Review Sentiment Analysis

## 📌 Overview
Classifies Amazon product reviews as positive or negative using TF-IDF + Logistic Regression, SVM, and a Neural Network with GloVe Word2Vec embeddings.

## 📂 Dataset
- **File:** `amazonreviews.tsv`
- **Target:** `label` (pos / neg)

## 🔍 What's Inside
- EDA — sentiment distribution, WordClouds (all / positive / negative reviews)
- NLTK tokenization + stopword removal
- Top 20 positive and negative words extracted
- **TF-IDF** vectorization for LR and SVM
- **GloVe (glove-wiki-gigaword-100)** embeddings for Neural Network
- Neural Network: `Dense(128, relu) → Dropout(0.5) → Dense(1, sigmoid)`
- 5-Fold StratifiedKFold cross-validation on Logistic Regression
- Final comparison — LR vs SVM vs NN

## 📊 Model Comparison
| Model | Result |
|-------|--------|
| Logistic Regression + TF-IDF | Strong, consistent CV results |
| SVM + TF-IDF | Best overall ✅ |
| Neural Network + Word2Vec | Good, needs more data |

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn` `nltk` `wordcloud` `tensorflow` `gensim`

---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| Recommendation System | `01_Recommendation_System.ipynb` |
| Time Series Forecasting | `02_Time_Series.ipynb` |
| NLP Sentiment Analysis | `03_NLP.ipynb` |

---

## 🛠️ How to Run

```bash
git clone https://github.com/Shivas28/ML-Portfolio.git
cd ML-Portfolio/06_Advanced_Topics
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
