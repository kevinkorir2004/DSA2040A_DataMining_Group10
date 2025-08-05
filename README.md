# DSA2040A Data Mining Group Project – Project Proposal

## Group 9 – Health Risk Prediction

### 📌 Project Title
**Health Risk Prediction Based on Lifestyle and Demographic Attributes**

### 👥 Group Members & Roles
- **Alfred (...)** – Visualization
- **Margaret (497)** – ETL
- **Kevin (656)** – ETL, Documentation
- **Bricole (...)** – Data Mining
- **Geoffrey (...)** – Dashboard

---

### 🎯 Project Overview
Chronic illnesses such as hypertension, diabetes, and cardiovascular disease pose major public health challenges. This project aims to **identify key demographic and lifestyle factors that influence an individual's risk of developing chronic illness**. By using synthetic health data that reflects real-world patterns, the project seeks to extract meaningful insights and predictive patterns using data mining techniques.

---

### ❓ Key Questions
- What are the most significant lifestyle and demographic contributors to chronic illness risk?
- Can individuals be grouped into risk segments using clustering?
- How accurately can we predict illness risk based on selected features?

---

### 🛠️ Proposed Methods and Techniques

- **ETL Pipeline**: Synthetic dataset generation → Cleaning → BMI computation → Encoding
- **Exploratory Analysis**: Statistical distributions, group comparisons, correlation analysis
- **Data Mining**:
  - **Classification**: Logistic regression, decision trees
  - **Clustering**: K-means to segment population into risk clusters
- **Visualization**: Interactive charts for dashboard and reporting

---

### 🧰 Tools & Libraries

- **Programming**: Python (Pandas, NumPy, Scikit-learn)
- **Visualization**: Seaborn, Matplotlib, Plotly
- **Dashboarding**: Jupyter Dash or Plotly Dash
- **Version Control**: GitHub

---

### 📅 Week 1 Deliverables

- ✅ Project topic: **Health Risk Prediction**
- ✅ Group formed and roles assigned
- ✅ Synthetic dataset generated
- ✅ This README.md as the official project proposal

### Week 2 Deliverables – ETL & Enrichment
✅ Cleaned and transformed the synthetic dataset
✅ Removed duplicates and handled missing values
✅ Created enriched features:
  .BMI category (e.g. Healthy, Overweight)
  .Age group bins
  .One-hot encoded categorical variables (e.g. smoking status, gender)

✅ Scaled numerical features for model readiness
✅ Saved cleaned data to data/transformed/health_cleaned.csv
✅ ETL updates documented in notebooks/1_extract_transform.ipynb

### Week 3 Focus:

- Correlation analysis via heatmaps to reveal strong feature relationships (e.g., weight ↔ BMI, age bins)
- Distribution plots for BMI and behavioral metrics to assess data spread and balance
- Group comparisons between obesity status, chronic illness, age brackets, and behavioral flags
- Toolset: pandas, matplotlib, seaborn, scikit-learn
- Added scaling, binning, and one-hot encoding during ETL to prepare features for mining

### Week 4 – Data Mining 

key data mining techniques on a synthetic health dataset:

* **Classification:** Logistic Regression, Decision Tree
* **Clustering:** K-Means, DBSCAN


## 1️⃣ Classification

### Techniques Used:

* **Logistic Regression**
* **Decision Tree Classifier**

### Goal:

Predict the presence of chronic illness based on patient data.

### Evaluation Metrics:

* **Accuracy**
* **Classification Report (Precision, Recall, F1-score)**

### Results:

* Logistic Regression and Decision Tree models both showed solid performance.
* Decision Tree offers interpretable decision paths.

### Interpretation:

Risk factors such as blood pressure, cholesterol, and smoking status strongly influence chronic illness prediction. The models enable proactive identification of at-risk individuals.


## 2️⃣ Clustering

### Techniques Used:

* **K-Means Clustering**
* **DBSCAN (Density-Based Spatial Clustering)**

### Goals:

* Group patients into meaningful health segments without using target labels.
* Uncover hidden patterns in the dataset.

### Evaluation Metrics:

* **K-Means:** Silhouette Score
* **DBSCAN:** Number of clusters & noise points

### Results:

* **K-Means:** Identified 3 distinct clusters with moderate silhouette score.
* **DBSCAN:** Revealed clusters with outliers handled as noise, based on density rather than centroid distance.

### Interpretation:

* K-Means grouped patients based on similar health profiles.
* DBSCAN was effective in detecting smaller dense groups and isolating outlier cases (potential anomalies or unique health patterns).


## 🛠️ Tools Used

* Python 3
* Jupyter Notebook (VS Code)
* Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`




##

---



### 📂 Repository Structure (Planned)

