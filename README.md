# Telecom Customer Churn Prediction

## Overview

This project predicts customer churn for a telecom company using supervised machine learning.
Customer churn occurs when users discontinue services, impacting revenue.
The goal is to identify high-risk customers early so businesses can implement retention strategies.


## Objectives

* Analyze customer demographics and service usage patterns.
* Build classification models to predict churn (Yes/No).
* Compare multiple ML algorithms for performance.
* Optimize evaluation metrics to reduce false negatives.
* Extract actionable insights for business decision-making.


## Dataset

* **Source:** IBM Telco Customer Churn Dataset
* **Records:** 7,043 customers
* **Features:** 20+ attributes including:

  * Tenure
  * MonthlyCharges
  * Contract Type
  * Internet Service
  * Payment Method
  * Total Charges


## Methodology

### Data Preprocessing

* Removed non-informative fields (`customerID`).
* Converted `TotalCharges` to numeric and handled hidden missing values.
* Applied **One-Hot Encoding** to categorical variables.
* Standardized numerical features using **StandardScaler**.
* Split dataset into **80:20 train-test sets**.

### Exploratory Data Analysis (EDA)

Key insights discovered:

* Month-to-month contracts show higher churn.
* Customers with shorter tenure are more likely to leave.
* Higher monthly charges correlate with churn risk.

### Models Implemented

* Logistic Regression (baseline, interpretable)
* K-Nearest Neighbors (distance-based learning)
* Random Forest (ensemble learning)
* Gradient Boosting (sequential optimization)

### Evaluation Metrics

Models were evaluated using:

* Recall (to capture actual churners)
* F1-Score (balance between precision and recall)
* ROC-AUC (classification separability)


## Results

**Gradient Boosting delivered the best performance:**

* ROC-AUC ≈ **0.84**
* Balanced recall and precision
* Strong generalization on unseen data

This model effectively identifies customers likely to churn.


## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib / Seaborn
* Jupyter Notebook / Google Colab


## Future Improvements

* Hyperparameter tuning for improved recall.
* Deployment using Streamlit for real-time predictions.
* Integration into CRM systems for automated retention alerts.

---

## 📌 Conclusion

This project demonstrates how machine learning can transform customer data into actionable business insights, helping organizations proactively retain customers and reduce revenue loss.
