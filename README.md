# 📊 World University Ranking Analysis (2011–2016)

A complete data cleaning, exploratory analysis, and machine‑learning project using the Times Higher Education (THE) dataset.

---

## 📁 Project Overview

This project analyzes global university rankings from 2011–2016.  
It includes:

- Automated data loading  
- Data cleaning & preprocessing  
- Feature engineering  
- Exploratory Data Analysis (EDA)  
- Machine Learning Models  
  - K‑Means Clustering  
  - Linear Regression  
  - Random Forest Regression  
- Visualizations for insights and model interpretation  

---

## 📂 Repository Structure

---

## 🧹 Data Cleaning & Preprocessing

### ✔️ Key Steps

- Corrected country name inconsistencies  
- Extracted top 200 universities per year  
- Removed "=" from ranking values  
- Converted numeric columns stored as strings  
- Cleaned:
  - `international_students` (% → float)
  - `female_male_ratio` (split + computed ratio)
  - `num_students` (removed commas)
  - `income`, `international`, `total_score` (converted to float)
- Normalized university names (removed native characters)
- Removed rows with missing values

Final cleaned dataset: **953 rows × 15 columns**

---

## 🔍 Exploratory Data Analysis (EDA)

### 📈 Pair Plot  
`![Pair Plot](images/pairplot.png)`

### 🔥 Correlation Heatmap  
`![Heatmap](images/heatmap.png)`

**Insights:**

- Teaching & Research strongly correlate with Total Score  
- Citations moderately correlate  
- International score has weak correlation  

---

## 🤖 Machine Learning Models

---

### 🎯 1. K‑Means Clustering

Features used:

- Teaching  
- Research  
- Citations  
- International  

`![K-Means Clusters](images/kmeans_clusters.png)`

**Cluster Meaning:**

- **Cluster 2** → Top‑tier universities  
- **Cluster 1** → Mid‑tier  
- **Cluster 0** → Lower‑tier  

---

### 📉 2. Linear Regression

Predicting **Total Score** using:

- Teaching  
- Research  
- Citations  

**Results:**

| Metric | Score |
|--------|--------|
| MSE | 2.54 |
| R² | 0.98 |

`![Linear Regression](images/linear_regression.png)`

---

### 🌲 3. Random Forest Regressor

**Results:**

| Metric | Score |
|--------|--------|
| MSE | 3.12 |
| R² | 0.98 |

`![Random Forest Importance](images/random_forest_importance.png)`

**Feature Importance:**

1. Teaching  
2. Research  
3. Citations  

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit‑Learn  
- Seaborn  
- Matplotlib  
- Unicodedata  

---

## 🚀 How to Run

```bash
git clone https://github.com/yourusername/university-ranking-analysis.git
cd university-ranking-analysis
pip install -r requirements.txt
jupyter notebook
If you want, I can also generate:

- a **requirements.txt**  
- a **project banner**  
- a **GitHub description**  
- or convert this README into a **professional portfolio project section**.

Just tell me what you want next.
