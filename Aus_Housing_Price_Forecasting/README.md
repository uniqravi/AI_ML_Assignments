# Bike Sharing Demand Forcasting
> In this project, We have built multiple regression model to predict number of demand of bike sharing in system.


## Table of Content
* [Problem  Statement](#problem-statement)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

 
The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

    - Which variables are significant in predicting the price of a house, and

    - How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.

## Business Goal:

We are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.
 
 ## Modeling :
 - Built Lasso & Ridge Regression model.
 - Used GridSearchCV to get optimal value of alpha
   
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

- Lasso model does feature selection and it also perform give good accuracy score.
- P value of model parameters are more significant compare to ridge model.
- recieved low p and low vif in less number of iteration.
- final list of best predictors are

*   Condition2 (posN)
*   OverallQual (10,9)
*   RoofMatl (WdShngl)
*   PoolQC (Ex,)
*   Neighborhood (StoneBr,NoRidge,Crawfor,NridgHt)
*   2ndFlrSF
*   1stFlrSF
*   BsmtExposure(Gd)
*   KitchenQual(Ex)
*   ExterQual(Ex)
*   BsmtQual(Ex)
*   BsmtQual(Ex)
*   OverallCond(3,4,8)
*   LotShape


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - 3.10
- Pandas - 1.5.0
- Numpy - 1.23.3
- Matplotlib - 3.6.0
- Seaborn- 0.12.0
- sklearn
- statsmodels

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact

Created by [@uniqravi] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->
