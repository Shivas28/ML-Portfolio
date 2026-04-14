# 🤖 Classical Machine Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)

> Implementation of core supervised learning algorithms across regression and classification tasks, with model comparison, hyperparameter tuning, and real-world datasets.

---

## 📚 Notebooks

# 🚗 Multiple Linear Regression — Toyota Corolla Price Prediction

## 📌 Overview
Predicts used car prices from the Toyota Corolla dataset by comparing three progressively simpler models and applying regularization techniques.

## 📂 Dataset
- **File:** `ToyotaCorolla - MLR.csv`
- **Target:** `Price` (in EUR)
- **Features:** Age, KM, Fuel Type, HP, Weight, CC, and more

## 🔍 What's Inside
- EDA — price distribution, correlation heatmap, Age vs Price scatter
- One-Hot Encoding on `Fuel_Type`
- **Model 1:** All features → best overall performance
- **Model 2:** Top 5 features (Age, KM, Weight, HP, CC)
- **Model 3:** Age + KM only → simplest model
- Ridge (L2) and Lasso (L1) regularization with StandardScaler
- Actual vs Predicted price plot

## 📊 Key Metrics
| Model | R² Score |
|-------|----------|
| All Features (M1) | Best |
| Top 5 Features (M2) | Moderate |
| Age + KM Only (M3) | Lowest |

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn`

---

# 🩺 Logistic Regression — Diabetes Prediction

## 📌 Overview
Binary classification model to predict diabetes risk using the Pima Indians dataset, with deployment-ready code included.

## 📂 Dataset
- **File:** `diabetes.csv`
- **Target:** `Outcome` (1 = Diabetic, 0 = Not Diabetic)
- **Features:** Glucose, BMI, Insulin, Blood Pressure, Age, and more

## 🔍 What's Inside
- EDA — histograms, boxplots, pairplot
- Zero-value imputation using column medians (Glucose, BMI, Insulin, etc.)
- StandardScaler normalization
- Logistic Regression training and evaluation
- Confusion matrix, classification report, ROC curve & AUC score
- Model saved using `joblib` (`.pkl` files)
- Streamlit deployment code included

## 📊 Key Metrics
- Accuracy, Precision, Recall, F1-Score
- ROC-AUC Score
- Train vs Test accuracy comparison

## 🛠️ Libraries
`pandas` `matplotlib` `seaborn` `scikit-learn` `joblib`

---

# 💊 Support Vector Machine — Pharma Drug Response Classification

## 📌 Overview
Classifies drug response in pharmaceutical industry data using SVM with multiple kernel comparisons and parameter tuning.

## 📂 Dataset
- **File:** `Pharma_Industry.csv`
- **Target:** `Drug Response`

## 🔍 What's Inside
- EDA — feature distributions, correlation heatmap, pairplot, class count
- StandardScaler preprocessing
- SVM with **Linear kernel** (baseline)
- SVM with **RBF kernel** — best performer
- SVM with **Polynomial kernel**
- C parameter tuning (0.1, 1, 10, 100) on RBF kernel
- Confusion matrix heatmap

## 📊 Kernel Comparison
| Kernel | Accuracy |
|--------|----------|
| Linear | 78% |
| RBF | 84% ✅ |
| Poly | 71% |

> RBF performed best — confirms the data is non-linearly separable.

## 🛠️ Libraries
`pandas` `matplotlib` `seaborn` `scikit-learn`

---

# 🫀 Decision Tree — Heart Disease Prediction

## 📌 Overview
Predicts the presence of heart disease using Decision Tree classifier with hyperparameter tuning via GridSearchCV.

## 📂 Dataset
- **File:** `heart_disease.xlsx`
- **Target:** `num` (1 = Disease, 0 = No Disease)

## 🔍 What's Inside
- Data cleaning — median imputation for `oldpeak`, boolean mapping for `exang`
- One-Hot Encoding on categorical columns (`sex`, `cp`, `thal`, etc.)
- StandardScaler on numerical features
- Decision Tree with **Gini** criterion (depth=6)
- Decision Tree with **Entropy** criterion (depth=4)
- **GridSearchCV** tuning — `max_depth`, `min_samples_split`, `criterion`
- Feature importance bar chart
- Full tree visualization with `plot_tree`

## 📊 Key Metrics
- Accuracy, Precision, Recall, F1-Score, ROC-AUC
- Best parameters from GridSearchCV

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn`

---

# 🔮 Random Forest — Glass Type Classification

## 📌 Overview
Multi-class classification of glass types using Random Forest, with SMOTE applied to handle severe class imbalance, and comparison against Bagging and AdaBoost.

## 📂 Dataset
- **File:** `glass.xlsx`
- **Target:** `Type` (7 glass categories)

## 🔍 What's Inside
- EDA — histograms, boxplots, correlation heatmap, pairplot
- Class imbalance detection (Type 6 had only 9 samples vs Type 2 with 76)
- **SMOTE** applied to balance classes before training
- StandardScaler normalization
- **Random Forest** vs **Bagging** vs **AdaBoost** comparison
- Full metrics — Accuracy, Precision, Recall, F1-Score

## 📊 Model Comparison
| Model | Accuracy |
|-------|----------|
| Random Forest | 92% ✅ |
| Bagging | 90% |
| AdaBoost | 86% |

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn` `imbalanced-learn`
---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| Multiple Linear Regression | `01_Multiple_Linear_Regression.ipynb` |
| Logistic Regression | `01_Logistic_Regression.ipynb` |
| Support Vector Machine | `02_SVM.ipynb` |
| Decision Tree | `03_Decision_Tree.ipynb` |
| Random Forest | `04_Random_Forest.ipynb` |

---

## 🛠️ How to Run

```bash
# Clone the repo
git clone https://github.com/Shivas28/ML-Portfolio.git

# Navigate to folder
cd ML-Portfolio/02_Classical_ML

# Launch Jupyter
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
