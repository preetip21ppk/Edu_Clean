# 🎓 EduCleanML: Data Cleaning & School Enrollment Analysis (US K-12 Dataset)

*Author:* Preeti Purnimaa Kannan  
*Affiliation:* M.S in Data Analytics Engineering — Northeastern University, Boston, USA  

---

## 🧠 Project Overview

*EduCleanML* is a comprehensive data analysis and machine learning project focused on cleaning, exploring, and modeling a large-scale *U.S. K–12 school dataset (2022–2023)*.  
The goal is to understand student enrollment patterns, address missing and inconsistent data, and develop predictive insights into *total enrollment* using regression and clustering techniques.

---

## 🚀 Objectives

- Perform large-scale data cleaning and preparation for a 100k+ row dataset  
- Handle missing data, duplicates, and inconsistencies  
- Conduct Exploratory Data Analysis (EDA) using *Seaborn* visualizations  
- Identify important features influencing school enrollment  
- Apply *Random Forest* and *XGBoost* regression for predictive modeling  
- Use *K-Means clustering* to group schools by demographic and resource patterns  

---

## 📂 Project Structure
EduCleanML/
│
├── data/
│ └── school.csv # Raw dataset (U.S. K-12 data)
│
├── notebooks/
│ └── PROJECT2_EDUCLEAN.ipynb # Core notebook / PDF analysis
│
├── results/
│ ├── correlation_heatmap.png # Feature correlation visualization
│ ├── enrollment_vs_stut_ratio.png # Scatterplot for key relationships
│ ├── school_type_distribution.png # Countplot for categorical feature
│ ├── fixed_school_clusters.png # Cluster visualization
│ └── histograms_boxplots/ # Distribution & outlier plots
│
├── models/
│ ├── random_forest_model.pkl
│ └── xgboost_model.pkl
│
├── requirements.txt # Python dependencies
│
└── README.md # Project documentation


---

## 🧹 Data Cleaning Process

- Dropped columns with *>90% missing values*  
- Imputed:
  - *Numeric columns:* Median  
  - *Categorical columns:* Mode  
- Standardized *ZIP codes, removed invalid **latitude/longitude*  
- Scaled numeric data using *Min–Max normalization*  
- Applied *Label Encoding* for categorical features  
- Ensured *total enrollment consistency* with grade-level sums  

---

## 🔍 Exploratory Data Analysis (EDA)

- *Histograms & Boxplots* → data distribution & outlier detection  
- *Scatterplots* → relationship between total enrollment & student–teacher ratio  
- *Heatmaps* → feature correlations  
- *Categorical Plots* → distribution across school types  

---

## 🧩 Machine Learning Models

| Model | Objective | Key Metric | Performance |
|-------|------------|------------|--------------|
| *Random Forest Regressor* | Feature importance & baseline model | R² = 0.96 | Excellent |
| *XGBoost Regressor* | Predict total enrollment | R² = *0.978* | Excellent |
| *K-Means Clustering* | Group schools by patterns | 3 clusters | Visualized |

### 🔑 Feature Importance (Top 5)

| Feature | Importance |
|----------|-------------|
| GSLO (Grade Start Level) | 0.57 |
| GSHI (Grade End Level) | 0.34 |
| SCHOOL_LEVEL | 0.08 |
| SCHOOL_TYPE_TEXT | 0.000004 |
| DIRECTCERT | 0.000002 |

---

## 📊 Evaluation Metrics

| Metric | Value |
|--------|--------|
| Mean Absolute Error | 0.433 |
| Mean Squared Error | 0.457 |
| R-Squared | *0.978* |

---

## 🧠 Insights

- *Enrollment strongly correlates* with grade-level ranges (GSLO, GSHI)  
- Schools with *broader grade spans* tend to have higher total enrollment  
- Minor influence from categorical variables such as school type or district  
- K-Means clustering reveals *3 key school behavior groups*  

---

## 🛠 Technologies Used

- *Python 3.9+*
- *Pandas, **NumPy, **Seaborn, **Matplotlib*
- *Scikit-learn, **XGBoost*
- *Jupyter Notebook / VS Code*

---

## 🧩 Future Enhancements

- Integrate *geospatial visualization* (Plotly/GeoPandas)  
- Add *interactive dashboard* using *Streamlit or Power BI*  
- Explore *deep learning regressors* for improved accuracy  
- Compare *Prophet/Greykite* models for time-based school trends  

---





---
