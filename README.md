# CreditRiskModeling
### Introduction
We know that If we applied for a credit card or loan, financial firms process the information before making a decision. This is because giving a loan can have a serious financial impact on their business. But how do they make a decision? This project aims to predict the probability of default(PD) and further to reduce risk and ensure profitability.

### Data
cr_loan2.csv

variables: 
person_age, person_income, person_home_ownership, person_emp_length, loan_intent, loan_grade, loan_amnt, loan_int_rate, loan_percent_income, cb_person_default_on_file, cb_person_cred_hist_length, loan_status

### Exploring and Preparing Loan Data
- Explore loan data set by cross tables and plots, which include histogram, scatter plot, boxplot, heatmap, pairplot.
- Delete 7 outliers
- Impute the null values
- One-hot encode the non-numeric columns
- Scaling
- Deal with imbalanced data
### Modeling
#### logistic Regression
- accuracy: 0.87
- recall: 0.87
- AUC: 0.8718
#### Decision Tree
- accuracy: 0.89
- recall: 0.89
- AUC: 0.8463
#### Random Forest
- accuracy: 0.90
- recall: 0.90
- AUC: 0.7910
#### XGBoost
- accuracy: 0.93
- recall: 0.93
- AUC: 0.8633

Based on the metrics above and the calibration curve, XGBoost model has a stong predictive performance.

### Credit Strategy
Develop a business strategy by setting various acceptance rate to maximize the estimate portfolio value
