# 🤖 Classical Machine Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)

> Implementation of core supervised learning algorithms across regression and classification tasks, with model comparison, hyperparameter tuning, and real-world datasets.

---

## 📚 Notebooks

### 📓 1. Multiple Linear Regression
- **Dataset:** Toyota Corolla
- **Goal:** Predict used car prices based on vehicle features
- **Techniques:** Three model variants (all features → top 5 → Age+KM only), OHE on `Fuel_Type`, Ridge & Lasso regularization, actual vs predicted visualization
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

### 📓 2. Logistic Regression
- **Dataset:** Diabetes (Pima Indians)
- **Goal:** Predict whether a patient has diabetes
- **Techniques:** Zero-value imputation with median, StandardScaler, ROC curve & AUC score, model saved with `joblib`, Streamlit deployment code included
- **Libraries:** Pandas, Matplotlib, Seaborn, Scikit-learn, Joblib

---

### 📓 3. Support Vector Machine (SVM)
- **Dataset:** Pharma Industry
- **Goal:** Classify drug response in pharmaceutical data
- **Techniques:** EDA with correlation heatmap & pairplot, Linear / RBF / Polynomial kernel comparison, C parameter tuning — RBF kernel achieved best accuracy (84%)
- **Libraries:** Pandas, Matplotlib, Seaborn, Scikit-learn

---

### 📓 4. Decision Tree
- **Dataset:** Heart Disease
- **Goal:** Predict presence of heart disease
- **Techniques:** Gini vs Entropy criterion comparison, GridSearchCV hyperparameter tuning (`max_depth`, `min_samples_split`), feature importance visualization, tree plot
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

### 📓 5. Random Forest
- **Dataset:** Glass (UCI)
- **Goal:** Classify glass types based on chemical composition
- **Techniques:** SMOTE for class imbalance, Random Forest vs Bagging vs AdaBoost comparison — Random Forest achieved best accuracy (92%)
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn

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
