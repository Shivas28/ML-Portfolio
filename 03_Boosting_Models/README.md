# ⚡ Boosting Models

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

> Advanced gradient boosting techniques benchmarked head-to-head with hyperparameter tuning.

---

## 📚 Notebooks

# ⚡ 1. LightGBM vs XGBoost — Diabetes Prediction

## 📌 Overview
Benchmarks LightGBM and XGBoost on the Diabetes dataset with GridSearchCV tuning, evaluating which model performs better for a medical classification task.

## 📂 Dataset
- **File:** `diabetes.csv`
- **Target:** `Outcome` (1 = Diabetic, 0 = Not Diabetic)

## 🔍 What's Inside
- EDA — histograms, KDE plots, boxplots, pairplot, class distribution
- Zero-value imputation with median for medical columns
- StandardScaler normalization
- **LightGBM** training + GridSearchCV tuning (`n_estimators`, `learning_rate`, `num_leaves`)
- **XGBoost** training + GridSearchCV tuning (`n_estimators`, `learning_rate`, `max_depth`)
- Side-by-side comparison — Accuracy, Precision, Recall, F1, ROC-AUC

## 📊 Model Comparison
| Model | Result |
|-------|--------|
| LightGBM | Fast training, competitive accuracy |
| XGBoost | Slightly better ROC-AUC ✅ |

> For this medical dataset, Recall is prioritized — missing a diabetic patient (false negative) is more costly than a false alarm.

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn` `lightgbm` `xgboost`

---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| LightGBM vs XGBoost | `01_LightGBM_vs_XGBoost.ipynb` |

---

## 🛠️ How to Run

```bash
git clone https://github.com/Shivas28/ML-Portfolio.git
cd ML-Portfolio/03_Boosting_Models
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
