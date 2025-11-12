# 🧠 MGNREGA Worker Participation Analysis using Machine Learning

## 📋 Overview
This project analyzes worker participation trends in the **Mahatma Gandhi National Rural Employment Guarantee Act (MGNREGA)** using various **machine learning models**.  
The goal is to identify factors influencing job card issuance and participation levels, and to classify regions based on worker activity.

The project explores large-scale MGNREGA datasets (2014–2023) covering multiple states in India and applies **regression, clustering, and classification** algorithms to uncover key insights and predictive patterns.

---

## 🔍 Abstract
The project investigates how workers enroll and participate in MGNREGA schemes. Using data on registered workers, job cards applied, and job cards issued, several machine learning techniques—such as **Linear Regression, K-Means, DBSCAN, XGBoost, Random Forest**, and **Logistic Regression**—were applied.

Results revealed that **job card applications**, **total registered workers**, and **female participation** are key predictors of worker engagement.  
The **Random Forest** model achieved the highest accuracy of **0.96**, indicating strong predictability in MGNREGA participation trends.

---

## 🎯 Objectives
1. Clean and preprocess raw MGNREGA data.  
2. Perform Exploratory Data Analysis (EDA) for insights.  
3. Predict issued job cards using regression models.  
4. Cluster states based on worker participation patterns.  
5. Classify regions into Low, Moderate, and High participation categories.  
6. Visualize trends and feature importance using graphs.  

---

## 🧩 Methodology

### 📁 Dataset
- **Shape:** 2,676,899 rows × 18 columns  
- **Time Period:** 2014–2023  
- **Geographical Coverage:** Multiple states, districts, blocks, and gram panchayats across India

Dataset from: https://indiadataportal.com/p/mgnrega-mahatma-gandhi-national-rural-employment-guarantee-act/r/mord-mgnrega_category_wise_worker-gp-yr-aaa

### 🧹 Preprocessing Steps
- Removed null and duplicate entries  
- Dropped irrelevant columns (e.g., IDs, GP names)  
- Created derived features such as `female_worker_proportion`  
- Label-encoded categorical features  
- Standardized numerical variables  

---

## ⚙️ Implementation

### 💻 Environment
- **Language:** Python  
- **IDE:** VS Code  
- **Libraries Used:**  
  `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`

### 🚀 Steps Performed
1. Loaded and cleaned the dataset  
2. Conducted EDA and visualization  
3. Applied regression, clustering, and classification models  
4. Evaluated model performance using R², RMSE, and Accuracy  
5. Visualized key trends and patterns  

---

## 🤖 Models Used

| Model | Type | Goal | Performance |
|-------|------|------|-------------|
| Simple Linear Regression | Regression | Predict active workers | R² = 0.64 |
| Multiple Linear Regression | Regression | Predict active workers using multiple features | R² = 0.87 |
| K-Means Clustering | Unsupervised | Cluster states by participation | 3 clusters (Low, Moderate, High) |
| DBSCAN | Unsupervised | Identify dense/outlier regions | 1 dense cluster + 69 outliers |
| XGBoost Regression | Regression | Predict issued job cards | R² = 0.90 |
| Random Forest Regression | Regression | Predict issued job cards | R² = 0.96 |
| Logistic Regression | Classification | Classify participation levels | Accuracy = 72% |

---

## 📊 Key Insights
- **Applied Jobcards** and **Total Registered Workers** are the strongest predictors of participation.  
- **Random Forest** and **XGBoost** gave the best performance (R² ≥ 0.90).  
- Data shows strong consistency across states, validating the scheme’s stable implementation.  
- Participation levels can be effectively categorized using logistic regression.  

---

## 🗺️ Future Work
1. Integrate **spatial visualization** using Folium and GeoPandas.  
2. Apply **time-series forecasting** for future participation predictions.  
3. Include **demographic and economic indicators** for richer insights.  

---

## 📚 References
1. Ghosh, R. (2013). *A Bird’s Eye View into Mahatma Gandhi National Rural Employment Guarantee Act.* World Bank Discussion Paper.  
2. Jayakumar, B., & Prabakar, S. (2024). *Leveraging Digital Innovation to Enhance MGNREGA’s Impact on Rural Empowerment.* IJCESEN.  
3. Arora, U., & Arora, G. (2023). *Analysis of the Impacts of MGNREGA using Spatial Data Analysis.* IIIT Delhi Repository.  
4. Han, J., & Kamber, M. *Data Mining: Concepts and Techniques.*  

---


## 🧾 License
This project is for academic and educational purposes only.
