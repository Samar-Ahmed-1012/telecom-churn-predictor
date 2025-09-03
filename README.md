Customer Churn Prediction Analysis
A comprehensive ML solution for telecom customer churn prediction. Features data analysis, multiple models (Logistic Regression, Random Forest, XGBoost), SHAP interpretability, business insights, and deployment-ready pipeline. Developed for Condantix Tech 2025  AI Internship.


📌 Objective
This project aims to analyze customer churn data to identify key factors influencing customer attrition and build predictive models to classify churned customers. The goal is to help businesses take proactive measures to retain customers by understanding patterns and drivers of churn.

📊 Dataset: https://www.kaggle.com/datasets/blastchar/telco-customer-churn
The dataset contains 7,043 customer records with 21 features, including:
the dataset: 
1. Demographic information: gender, SeniorCitizen, Partner, Dependents
2. Account details: tenure, Contract, PaperlessBilling, PaymentMethod
3. Service usage: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
4. Charges: MonthlyCharges, TotalCharges
5. Target variable: Churn (binary: Yes/No)

Data Preprocessing
 - Converted TotalCharges from string to numeric (11 missing values handled via mean imputation).
 - Encoded categorical variables using one-hot encoding (resulting in 7,072 features after encoding).
 - Addressed class imbalance (Churn rate: 26.54%).


🧠 Models Used
1. Logistic Regression
2. Random Forest
3. XGBoost
4. LightGBM
5. CatBoost

Techniques Applied
Class imbalance handling: SMOTE oversampling
Hyperparameter tuning: GridSearchCV
Feature importance analysis: SHAP values
Model evaluation: Accuracy, Precision, Recall, F1-score, ROC-AUC

🔍 Key Findings
1. Top Features Influencing Churn
2. Tenure: Longer tenure reduces churn risk.
3. Contract type: Month-to-month contracts have higher churn.
4. Payment method: Electronic checks are associated with higher churn.
5. Monthly charges: Higher charges correlate with increased churn.
6. Online security & tech support: Absence of these services increases churn.

2. Model Performance
 - Best model: XGBoost achieved the highest ROC-AUC (0.86) and F1-score (0.62).
 - Logistic Regression performed poorly due to class imbalance.
 - Oversampling (SMOTE) improved recall for minority class (churned customers).

3. Business Insights
 - Customers with long-term contracts are more loyal.
 - Senior citizens are more likely to churn.
 - High monthly charges without corresponding services (e.g., tech support) lead to dissatisfaction.

🛠️ Tools & Libraries
1. Python
2. Pandas, NumPy
3. Scikit-learn, XGBoost
4. SHAP (for explainable AI)
5. Imbalanced-learn (SMOTE)
6. Matplotlib, Seaborn

📈 Recommendations
 - Targeted retention programs for high-risk groups (e.g., month-to-month contracts).
 - Offer incentives for long-term contracts.
 - Improve customer service (e.g., tech support, online security).
 - Review pricing strategies for high-charge plans.

👨‍💻 Author
Developed as part of a data science project to predict customer churn and derive actionable insights.














