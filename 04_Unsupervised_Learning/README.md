# 🔍 Unsupervised Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

> Dimensionality reduction and clustering techniques to discover hidden patterns without labeled data.

---

## 📚 Notebooks

# 🍷 1. PCA — Wine Dataset Dimensionality Reduction

## 📌 Overview
Applies PCA to reduce 13 wine features to 2 principal components, then compares K-Means clustering performance on original vs PCA-transformed data.

## 📂 Dataset
- **File:** `wine.csv`
- **Target:** `Type` (3 wine categories)

## 🔍 What's Inside
- EDA — histograms, boxplots, correlation heatmap, pairplot
- StandardScaler before PCA (required — features must be same scale)
- Scree plot + cumulative variance plot → 2 components selected
- PCA scatter plot colored by wine type
- K-Means (k=3) on original data vs PCA data
- Silhouette Score and Davies-Bouldin Score comparison

## 📊 Clustering Comparison
| Dataset | Silhouette Score | Davies-Bouldin |
|---------|-----------------|----------------|
| Original | Computed | Computed |
| PCA (2 components) | Slightly Better ✅ | Lower ✅ |

> PCA made cluster boundaries clearer and easier to visualize.

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn`

---

# ✈️ 2. Clustering — EastWest Airlines Customer Segmentation

## 📌 Overview
Segments airline customers into groups using K-Means, DBSCAN, and Hierarchical Clustering to support targeted marketing strategies.

## 📂 Dataset
- **File:** `EastWestAirlines.xlsx`
- **Sheet:** `data`

## 🔍 What's Inside
- EDA — histograms, boxplots, correlation heatmap
- StandardScaler (Balance, Bonus_miles, Days_since_enroll had high variance)
- **K-Means** — Elbow Method → k=4 selected
- **DBSCAN** — K-Distance graph for eps tuning, noise points identified
- **Hierarchical Clustering** — Dendrogram on 100-row sample, Ward linkage
- Silhouette Score comparison across all three methods

## 📊 Algorithm Comparison
| Algorithm | Result |
|-----------|--------|
| K-Means | Best Silhouette Score ✅ |
| DBSCAN | Found noise/outlier customers |
| Hierarchical | Good structure visualization |

> K-Means clusters can directly guide airline marketing — frequent flyers vs inactive members need very different offers.

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn` `scikit-learn` `scipy`

---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| PCA + Clustering Comparison | `01_PCA.ipynb` |
| K-Means, DBSCAN, Hierarchical | `02_Clustering.ipynb` |

---

## 🛠️ How to Run

```bash
git clone https://github.com/Shivas28/ML-Portfolio.git
cd ML-Portfolio/04_Unsupervised_Learning
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
