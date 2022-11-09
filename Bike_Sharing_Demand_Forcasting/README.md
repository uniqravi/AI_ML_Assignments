# Lending Club Case Study
> In this project, We uses basic EDA techniques and developed a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
A consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
   1. If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company </b>
   2. If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment. 

This case study is about to solve consumer finance company problem and helping company to take decision for approval of loan application.When a person applies for a loan, there are two types of decisions that could be taken by the company: If the company approves the loan, there are 3 possible scenarios described below:

1. Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

2. Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

3. Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 
    
The dataset contains the complete loan data for all loans issued through the time period 2007 t0 2011.
DataSet and it's attributes descrption can be accessed using below link : 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- we found out that 50% loan application belong to top 6 state out of 50 state.Name of top 6 states are the CA,NY,FL,TX,NJ,IL and 80% loan applications belong to 17 states and FL state provide most default loan and most fully paid loans are from TX state.
- we obeserve as employement term increases, they are less likeyly to apply loan application
- Low number of loan applications get filed in Jan month, increase as it reaches towards end of financial year. I think In Us bank likely to close maximum application before finacial year.
- higher intrest rate loan is more likely to end up with charged off.
- From Box plot of annual income, Q3 value of charged off loan is lower than fully paid loan. It means good income persons are more likely to close loan as fully paid.
- From Box plot of Debt to income ratio, q1, median, and q3 having larger value in charged off loan. higher debt to income ratio is not good. 
- loan applications of people who did not mentioned empoyee length with home ownership rent are more risky application.
- Generally it evident that People with 'other' Home ownership are more risky no matter what they belong to any income category.
- there is highly chance that loan application of very low income are going to be defaulter.
- Similary people with mortage home ownership are likely to complete loan succesfully.
- Median of installment of each category of not paying people is higher than paid off peiple.Same thing happend with third quartile. It means people each category with lower installment is more safe.
- bigger debt to income ratio and higher number of public bankrupt means more chance to become loan defaulter.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - 3.10
- Pandas - 1.5.0
- Numpy - 1.23.3
- Matplotlib - 3.6.0
- Seaborn- 0.12.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- This project was inspired to take fair understanding of how to solve real business problem using basic EDA techniques.


## Contact

Created by [@uniqravi] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->
