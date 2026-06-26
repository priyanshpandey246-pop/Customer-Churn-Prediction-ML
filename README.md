#  Customer Churn Prediction and Customer Segmentation using Machine Learning

##  Project Overview

Customer churn is a critical business problem where companies lose customers to competitors. 
This project aims to build a Machine Learning model to predict customer churn and identify high-risk customer segments using clustering techniques. 

The objective is to help businesses proactively identify customers who are likely to leave and design targeted retention strategies.


## Dataset Description

The project uses the Telco Customer Churn dataset, which contains:

- Customer demographic information
- Service subscription details
- Billing and payment information
- Contract type and tenure
- Target variable: Churn (Yes/No)

The dataset provides insights into customer behavior and service usage patterns.

---

##  Project Workflow

### 1️ Data Preprocessing
- Loaded dataset using Pandas
- Handled missing values
- Converted categorical variables using encoding techniques
- Performed train-test split for model validation

---

### 2️ Exploratory Data Analysis (EDA)

Performed detailed analysis to understand customer behavior:

- Analyzed overall churn distribution
- Visualized tenure vs churn relationship
- Studied impact of Monthly Charges and Contract Type
- Used boxplots and scatterplots to identify behavioral patterns

EDA revealed that customers with lower tenure and higher monthly charges tend to churn more frequently.

---

### 3️ Churn Prediction Modeling

Implemented and compared multiple classification models:

- Logistic Regression
- Random Forest Classifier

###  Model Evaluation Metrics:
- Accuracy (~80%)
- Confusion Matrix
- Precision, Recall, F1-score
- ROC-AUC Score (0.83)

The Random Forest model performed better and demonstrated strong class separation capability.

---

### 4️ Threshold Optimization

Since churn prediction is a recall-sensitive problem, classification threshold was tuned to improve churn detection.

This helped reduce false negatives and improve business impact.

---

### 5️ Feature Importance Analysis

Random Forest feature importance analysis identified key churn drivers:

- Tenure
- Monthly Charges
- Contract Type
- Total Charges

These features significantly influence customer churn probability.

---

### 6️ Customer Segmentation (K-Means Clustering)

Applied K-Means clustering to segment customers into distinct groups based on behavioral features.

- Identified high-risk churn segment
- Compared segment-wise tenure and billing characteristics
- Visualized clusters using scatterplots and boxplots

Segmentation provides actionable insights for targeted retention campaigns.

---

## 📈 Key Insights

- Customers with lower tenure are more likely to churn.
- Higher monthly charges increase churn probability.
- Month-to-month contract customers show higher churn rates.
- A specific cluster exhibited significantly higher churn behavior.
- Threshold tuning improved churn recall performance.

---

##  Business Impact

The model enables:

- Early identification of high-risk customers
- Data-driven retention strategies
- Targeted marketing campaigns
- Improved customer lifetime value

This solution can help telecom businesses reduce churn and increase profitability.

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

##  Future Improvements

- Hyperparameter tuning for performance improvement
- Deployment using Streamlit or Flask
- Integration with real-time customer data
- Advanced explainability using SHAP values

---

##  Conclusion

This project successfully combines supervised learning for churn prediction and unsupervised learning for customer segmentation. The model achieved strong predictive performance (ROC-AUC 0.83) and provided meaningful business insights that can help organizations design effective retention strategies.
