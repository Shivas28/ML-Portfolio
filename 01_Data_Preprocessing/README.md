# 🧹 Data Preprocessing

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

> Foundational techniques for cleaning, structuring, and preparing raw datasets for machine learning models.

---

## 📚 Notebooks

### 📓 1. Data Transformations
- **Dataset:** Adult / Census Income
- **Goal:** Clean and prepare demographic data for predictive modeling
- **Techniques:**
  - Missing value detection and mode imputation (`workclass`, `occupation`, `native_country`)
  - Feature separation — continuous vs. categorical columns
  - Scaling — StandardScaler (mean=0, std=1) and MinMaxScaler ([0,1] range)
  - Encoding — LabelEncoder for high-cardinality columns, OneHotEncoder for `sex`
  - Feature Engineering — `capital_net` (gain − loss), age binning into `Young/Middle/Senior`, log transformation on skewed `capital_gain`
- **Libraries:** Pandas, NumPy, Scikit-learn

---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| Feature Engineering & Cleaning | `01_Data_Transformations.ipynb` |

---

## 🛠️ How to Run

```bash
# Clone the repo
git clone https://github.com/Shivas28/ML-Portfolio.git

# Navigate to folder
cd ML-Portfolio/01_Data_Preprocessing

# Launch Jupyter
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
