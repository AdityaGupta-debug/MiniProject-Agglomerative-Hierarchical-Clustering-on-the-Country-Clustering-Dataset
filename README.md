# 🌍 Agglomerative Hierarchical Clustering on Country Data

This project demonstrates how to apply **Agglomerative Hierarchical Clustering** to group countries based on their socio-economic indicators using the [Country Clustering Dataset](https://www.kaggle.com/rohan0301/unsupervised-learning-on-country-data). The goal is to uncover hidden patterns and clusters among countries using unsupervised learning and visualize them in 2D space.

---

## 📊 Dataset Description

The dataset contains socio-economic indicators for 167 countries. Each row represents a country, and the features include various normalized indicators such as health, income, and imports.

### 🔍 Features:
- `child_mortality` – Deaths of children under 5 years per 1000 live births  
- `exports` – Exports of goods and services (% of GDP)  
- `health` – Health expenditure (% of GDP)  
- `imports` – Imports of goods and services (% of GDP)  
- `income` – Net income per person  
- `inflation` – Annual inflation rate  
- `life_expec` – Life expectancy  
- `total_fer` – Fertility rate  
- `gdpp` – GDP per capita

---

## 🧠 Techniques Used

- **Data Preprocessing**
  - Standardization using `StandardScaler`
- **Dimensionality Reduction**
  - Applied **PCA (Principal Component Analysis)** to reduce high-dimensional features to 2D for visualization.
- **Clustering**
  - Used **Agglomerative Hierarchical Clustering** (with Ward linkage and Euclidean distance) to cluster countries.
- **Visualization**
  - Dendrogram to show the hierarchy of merges
  - Scatter plot of 2D PCA components with cluster coloring

---

## 📈 Results

- PCA successfully reduced dimensions while preserving the structure of the data.
- Dendrogram helped determine the optimal number of clusters visually.
- Clustering revealed meaningful groupings of countries with similar development indicators.
- Final clusters were visualized using PCA-reduced 2D plots.

---

## 📌 How to Run

1. Clone this repository
2. Download the dataset from [here](https://www.kaggle.com/rohan0301/unsupervised-learning-on-country-data)
3. Install required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy
