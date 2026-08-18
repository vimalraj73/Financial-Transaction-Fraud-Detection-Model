# 📈 Fraud Detection Model in Financial Transactions

## 📰 Project Description

This is a capstone machine learning project focused on detecting fraudulent financial transactions using **Random Forest**.

The project was initially developed using a smaller dataset during my Data Science course and was later extended to the complete **6.36 million-row synthetic transaction dataset** for final model development and evaluation.

A **Power BI dashboard** was also created to visualize fraud patterns, transaction behavior, and key financial insights.

---

## 👤 Project Author

**Vimal Raj R**  
GitHub: [VimalRaj73](https://github.com/VimalRaj73)  
LinkedIn: [Vimal Raj R](https://www.linkedin.com/in/vimalraj73/)

---

## 💡 Project Context

This project demonstrates practical applications of **data preprocessing, feature engineering, machine learning, and business intelligence**.

The project focuses on handling an imbalanced fraud dataset, building a preprocessing pipeline using **ColumnTransformer**, evaluating multiple feature configurations, and analyzing the factors contributing to fraud predictions.

---

## 📊 Dataset

The project uses the **PaySim synthetic financial transaction dataset**, containing **6,362,620 transactions**.

The dataset is not included in this repository due to its large file size.

🔗 **Dataset:** [Fraudulent Transactions Dataset on Kaggle](https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset)

---

## 🎯 Project Overview & Goal

The objective is to classify financial transactions as:

- **1 → Fraudulent**
- **0 → Legitimate**

The final model was developed using the complete **6,362,620 transaction dataset** and evaluated using metrics such as **Precision, Recall, F1-Score, ROC-AUC, and PR-AUC**.

---

## 🛠️ Tools & Libraries

### 🧰 Python Stack

- **Pandas:** Data cleaning and feature engineering
- **NumPy:** Numerical computations
- **Scikit-learn:** Preprocessing, Random Forest, and model evaluation
- **Imbalanced-learn:** Machine learning pipeline
- **Matplotlib & Seaborn:** Data visualization

### 📊 BI & Visualization

- **Power BI:** Interactive fraud and transaction analysis

---

## 📝 Project Methodology

### 1. Data Preparation

The project uses a **6.36 million-row synthetic financial transaction dataset**.

Data preparation included:

- Data type and missing-value analysis
- Class imbalance analysis
- Removal of irrelevant identifier columns
- Stratified train-test splitting

### 2. Feature Engineering

Created transaction-based features including:

- **Hour_of_Day**
- **Day_of_Week**
- **ErrorBalanceOrg**
- **ErrorBalanceDest**

These features were created to capture transaction timing and inconsistencies between transaction amounts and account balances.

### 3. Modeling Pipeline

A **ColumnTransformer** was used for preprocessing:

- **StandardScaler** for numerical features
- **OneHotEncoder** for transaction type

The preprocessing steps and **RandomForestClassifier** were combined into a single pipeline.

### 4. Model Evaluation

Different feature configurations were evaluated to investigate the contribution of engineered and post-transaction features.

Model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Precision-Recall AUC
- Confusion Matrix

---

## 📊 Results

### Final Model Performance

> **Update these values with the final results from the 6.36M-row model.**

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 100.00% |
| **Precision (Fraud)** | 100.00% |
| **Recall (Fraud)** | 100.00% |
| **F1-Score (Fraud)** | 100.00% |
| **AUC-ROC** | 0.9991 |
| **PR-AUC** | 0.9985 

Because fraud transactions represent a small portion of the dataset, **Precision, Recall, F1-Score, ROC-AUC, and PR-AUC** were emphasized rather than accuracy alone.

---

## 📈 Power BI Dashboard Highlights

-The dashboard provides a high-level "Transaction Overview" of all business activity.

-It displays key performance indicators (KPIs) like total transaction volume, total fraud amount, and total transaction counts.

-A donut chart visually breaks down the proportion of all transaction types (like payments, transfers, etc.).

-An area chart tracks the trend of total transaction volume over time.

-The report contains a second, dedicated "Fraud Deep Dive" page that is filtered to only show fraudulent transactions.

-This fraud page features a bar chart to compare the total fraudulent amount for each specific transaction type.

-It also includes a table that lists the top 10 largest fraudulent transactions to pinpoint the highest-value cases.

---

## ⚠️ Dataset Limitation

The dataset is **synthetic/simulated** and therefore the model results should not be interpreted as production-level banking fraud performance.

---

## ✨ Key Learning

This project provided hands-on experience with **large-scale data analysis, feature engineering, imbalanced classification, preprocessing pipelines, model evaluation, and Power BI dashboard development**.
