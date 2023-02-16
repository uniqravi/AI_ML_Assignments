# Telecome Churn Prediction


In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 
15-25% annual churn rate.

Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.


## Problem Statement :

In this case study our main goal is to solve customer churning problem of telecom company using multiple machine learning algorithms based on their past months usages. 

Problem statement can be defined into two parts

- Since Telecom company wants to retain high valued customers and such customers are revenue generator, so on time prediction is very important. Company wants strategy to identify high value customer.

- Company also want to know important factors which is strong indicator of churning.

## Notebook Contents

It is binary classfication problem and This notebook covers following topics :

- Missing Value Treatment : Removed Features which having larger than 73% missing values and replace with median rest of dataset missing value.
- Exploratory Data Analysis
- Outlier Detection and Treatment : Replace higher extreme and lower extreme with q3+0.99IQR and q1-0.99IQR.
- High Valued Customer Detection using KMean Clustering :Used Hopkin methods to see that dataset contains cluster or not and used silhoutte score to identify best number of cluster.
- Train multiple model & Hiperparmeter Tuning : Used AdaboostingClassifier, GradientBoostingClassfier, RandomForestClassifier, XGB, Logistic Regression.Used GridSearchCV to tune hyperparameters.
- Finding Most Important Features 
- Comparing different multiple ML models with AUC score and Chosen Best One.

## Conclustion

- Total Incoming call of last month reduced by 7% to 11%, It is strogest indicator that customer is going to churn.
- Decreasing of Last Day Recharge Amount is second strogest indicator.
- Other Indicator are reducing total recharge amount, high gap from last recharge in month etc.

## Library Used
- Python - 3.10
- Pandas - 1.5.0
- Numpy - 1.23.3
- Matplotlib - 3.6.0
- Seaborn- 0.12.0
- sklearn 
- statsmodels

