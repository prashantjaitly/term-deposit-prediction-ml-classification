# Term Deposit Prediction & Machine Learning Classification

![Status](https://img.shields.io/badge/Status-Completed-success)
![Tech](https://img.shields.io/badge/Stack-Python%20|%20Scikit--Learn%20|%20Pandas-orange)
![Metric](https://img.shields.io/badge/Accuracy-90.4%25-green)

## 📌 Project Overview
A machine learning classification project designed to optimize marketing campaigns for a banking institution. The model predicts whether a client will subscribe to a term deposit based on demographic and behavioral data (Age, Job, Balance, Call Duration).

The goal is to replace "Cold Calling" with **"Propensity Modelling"**, identifying high-probability leads to improve conversion rates and reduce operational costs.

## 🎯 Business Objectives
1.  **Optimize Marketing ROI:** Target only customers with a high probability of subscription (predicted 'Yes').
2.  **Feature Importance:** Identify key drivers of conversion (e.g., Call Duration, Previous Campaign Outcome).
3.  **Model Benchmarking:** Compare linear baselines (Logistic Regression) vs. non-linear classifiers (Decision Trees).

## 🛠 Tech Stack & Methodology
* **Python:** Primary language for analysis and modelling.
* **Pandas & NumPy:** Data cleaning and manipulation.
* **Seaborn & Matplotlib:** Exploratory Data Analysis (EDA) to visualize trends.
* **Scikit-Learn:**
    * **Preprocessing:** One-Hot Encoding for categorical variables.
    * **Models:** Logistic Regression, Decision Tree Classifier.
    * **Evaluation:** Accuracy Score, Confusion Matrix, Classification Report.

---

## 📊 Model Performance & Insights

### 🔹 1. Algorithm Comparison
The **Decision Tree Classifier** significantly outperformed the Logistic Regression baseline, proving that the relationships between customer features and subscription are non-linear.

| Model | Accuracy Score | Verdict |
| :--- | :--- | :--- |
| **Logistic Regression** | 88.63% | Baseline |
| **Decision Tree** | **90.43%** | **Selected Model** |

### 🔹 2. Key Business Insights (EDA)
* **Call Duration:** This is the strongest predictor. Calls lasting longer than average show a exponentially higher conversion rate.
* **Job Profile:** 'Students' and 'Retired' individuals showed higher subscription rates compared to 'Blue-collar' workers.
* **Seasonality:** Engagement spikes in specific months (May), suggesting seasonal campaign timing is crucial.

### 🔹 3. Correlation Analysis
The analysis identified strong correlations between **Duration** and **Subscription Success**, validating the feature selection strategy.
![Model Performance](model_performance.JPG)

---

## 📂 Repository Structure
* [01_term_deposit_prediction.ipynb](01_term_deposit_prediction.ipynb): Complete Python code (Data Cleaning -> EDA -> Modeling).
* [02_bank_marketing_data.csv](02_bank_marketing_data.csv): Historical dataset used for training.
* `model_performance.JPG`: Visualization of results.
