## Assignment_House-Price-Prediction
## Table of Contents
1. Description of Project
2. Technologies Used
3. Steps followed during analysis
4. conclusion
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

 # Business Goal 

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

# The company wants to know:

Which variables are significant in predicting the price of a house, and

How well those variables describe the price of a house.

 

Also, determine the optimal value of lambda for ridge and lasso regression.


Assignment Part-II

Question 1

What is the optimal value of alpha for ridge and lasso regression? What will be the changes in the model if you choose double the value of alpha for both ridge and lasso? What will be the most important predictor variables after the change is implemented?

 

Question 2

You have determined the optimal value of lambda for ridge and lasso regression during the assignment. Now, which one will you choose to apply and why?

 

Question 3

After building the model, you realised that the five most important predictor variables in the lasso model are not available in the incoming data. You will now have to create another model excluding the five most important predictor variables. Which are the five most important predictor variables now?

 

Question 4

How can you make sure that a model is robust and generalisable? What are the implications of the same for the accuracy of the model and why?

 



## Technologies Used
-  pandas - 1.3.4
-  numpy - 1.20.3
-  seaborn - 0.11.2
-  matplotlib : 3.4.3
-  stasmodel- 0.12.2
-  sklearn- 0.24.2

## Steps followed during analysis
-  Step 1: Reading and Understanding the data
-  Step 2: Data visualization and outliers detection (if any)
-  Step 3: Data preparation
-  Step 4: Splitting the data into training and test sets
-  Step 5: Rescaling the variables
-  Step 6: Making Ridge and Lasso Regression models
-  Step 7: Making predictions using the test dataset with our model
-  Step 8: Model Evaluation
-  Step 9: Conclusion

## Conclusion (Ridge Regression):

According to the Ridge Regression model top 5 features which affect the price of the houses are:
1. GrLivArea: Above grade (ground) living area square feet
2. 1stFlrSF: First Floor square feet
3. 2ndFlrSF: Second floor square feet
4. YearBuilt: Number of years from original construction date to present year
5. OverallCond: Rates the overall condition of the house

## Conclusion (Lasso Regression):
According to the Lasso Regression model top 5 features which affect the price of the houses are:
1. GrLivArea: Above grade (ground) living area square feet
2. YearBuilt: Number of years from original construction date to present year
3. TotalBsmtSF: Total square feet of basement area
4. OverallCond: Rates the overall condition of the house
5. OverallQual: Rates the overall material and finish of the house


How well Model describe the price of a house.

The R-squared value on the test data for Ridge and Lasso Regression are given below

 Ridge - 0.893
 Lasso - 0.876

Since we have decent value of R squared our models can very well predict the price of houses
the difference in the r squared values of train and test data is not much so we can say that issue of overfitting is resolved.

The optimal lambda value in case of Ridge and Lasso Regression are below:
Ridge - 2.0
Lasso - 0.0001 

When the market value of the property is lower than the Predicted Sale Price, its the time to buy.


## Contact
Created by [@VipinJaguri] - feel free to contact me!
