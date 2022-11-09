# Bike Sharing Demand Forcasting
> In this project, We have built multiple regression model to predict number of demand of bike sharing in system.


## Table of Content
* [Problem  Statement](#problem-statement)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

    - Which variables are significant in predicting the demand for shared bikes.
    - How well those variables describe the bike demands

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

## Business Goal:

Building the model which will predict the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

## EDA Analysis :

 - This Bike Sharing Data consists 16 columns. The 'cnt' variable indicates the total number of bike rentals, including both casual and registered.So 'cnt' has been used as target variable and dropped casual and registered columns. 
 - Continuous Variable Analysis
   - There are Humidity, Windseepd, Temp and Atemp are continous varible in dataset.
   - temp and aTemp is higly linear to each other. 
 - Categorical Varible Analysis :
   - There is a low demand in Spring Season compared to summer, fall and winter. Generally,bike sharing demand remain high in summer and fall season.
   - Popularity of Bike Sharing demand is increasing. Trend is visible. There is a demand increase in 2019 compared to past year 2018.
   - From starting month to till 10th, In general demand increases then it starts to decline till Jan.
   - Median of holiday and first Q1 is less than compared to non-holiday median and Q1.
   - There is very low demand in snow season and no demand in heavy rainy season.
 
 ## Modeling :
 - Built Linear Regression model.
   
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

1. This case study is about to solve problem of forcasting of demand basis of given data.
2. During EDA, we use different plots to understand distribution of data, to understand relation b/w features in term how much they are corelated to each other. also performed such activity which determines linear dependent features to target variable.
3. Then we performed preprocessing step before start modeling. In this step we split the data into train and test and use standard scale to scale the continuous columns.
4. In model building , initally we followed traditional methods, first we choosed all features to build model. then we varify significane label by looking at P value of each features.
5. we use RFE to select top 17 features then we kept remvoing single feature in every try which come across below situation.
  - Remove first high VIF and High P value.
  - Keep Removing first Low VIF and High P value.
  - then finally Removing high VIF and low p value.
6. We also use adavance feature selection technique which is lasso. I know lasso can be used both purpose l1 regularization and model feature selection. I felt this model perfomed better than earlier point 5 technique.
7. I also performed an experiment. What I found we are building model with only two value of year 2018 and 2019 to follow the trend. Big Question is that if I am Building this model for 2020 , will this model behave correctly because we do not have corresponding encode value of year 2020. So follow trend I used lag data for previous four days. because yt follows yt-1 or yt-2 or yt-3 or yt-3. 
8. When I created model with this, these is no problem of overfit problem. Model bahaved much more correctly for test data.
9. It is somewhat time-series analysis like breaking components into trend, seasonal and errors. 

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
