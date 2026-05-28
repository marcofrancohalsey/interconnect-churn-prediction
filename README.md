# Customer Churn Prediction for Interconnect

### Overview

This project develops a machine learning model to predict customer churn at Interconnect using contract, billing, internet service, phone service, and customer information. The objective is to identify customers at risk of canceling the service in order to support retention strategies such as promotions or special plans. ROC-AUC is used as the main evaluation metric, with a target score of 0.88 on the test set.

### Data

The analysis uses four datasets containing information from 7,043 customers, including subscribed services, payment methods, billing history, customer information, and churn status.

### Methodology

- Preprocess and merge the datasets into a single dataframe.
- Perform exploratory data analysis to identify churn patterns.
- Create derived variables related to tenure and subscribed services.
- Train and evaluate classification models using ROC-AUC as the main metric.
- Compare the final model against a dummy baseline.

### Results

- Customers with month-to-month contracts, electronic check payments, fiber optic service, and lower tenure show higher churn rates.
- Customer tenure is one of the variables most strongly related to churn.
- The dummy model achieves a ROC-AUC of 0.5.
- CatBoostClassifier reaches a ROC-AUC of 0.9253 on the test set, surpassing the project target of 0.88 and demonstrating that the model is viable for identifying customers at risk of churn.

### Tools

Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, CatBoost
