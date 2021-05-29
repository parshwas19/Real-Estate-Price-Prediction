# Real-Estate-Price-Prediction
----
This is a Real Estate Price Prediction Model which I built using different Regression techniques.
As the name suggests this model is trained and tested in such a way that it predicts price of a house given some basic features.
I have used Boston state's Real estate data which is available on 'UCI Machine Learning repository'. 

The following steps are performed to build this model: <br/>
For splitting data into training and testing purposes, I have used Stratified Sampling. <br/>
Then I took a quick look by mapping co-relations of label with various features. <br/>  <br/>
Features: <br/>
    1. CRIM      per capita crime rate by town  <br/>
    2. ZN        proportion of residential land zoned for lots over 
                 25,000 sq.ft.  <br/>
    3. INDUS     proportion of non-retail business acres per town <br/>
    4. CHAS      Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)  <br/>
    5. NOX       nitric oxides concentration (parts per 10 million)  <br/>
    6. RM        average number of rooms per dwelling  <br/>
    7. AGE       proportion of owner-occupied units built prior to 1940  <br/>
    8. DIS       weighted distances to five Boston employment centres  <br/>
    9. RAD       index of accessibility to radial highways  <br/>
    10. TAX      full-value property-tax rate per $10,000  <br/>
    11. PTRATIO  pupil-teacher ratio by town <br/>
    12. B        1000(Bk - 0.63)^2 where Bk is the proportion of blacks 
                 by town <br/>
    13. LSTAT    % lower status of the population   <br/><br/>
Label(House Price) <br/>
    MEDV:    Median value of owner-occupied homes in $1000's <br/>

After that I differentiated features and labels into two different variables.<br/>
Then created an Imputer to perform tasks like: Filling the missing values (with median) and Feature Scaling(used Standardization technique for feature scaling). <br/>
For better evaluation technique I used Cross Validation on Training data.<br/> 
For selecting a desired model I tried 3 Regression techniques: Linear Regression, Decisin Tree Regressor & Random Forest Regressor. <br/> 

 <b>R square(coefficient of determination) regression score function:-</b>
Best possible score is 1.0 and it can be negative (because the model can be arbitrarily worse). A constant model that always predicts the expected value of y, disregarding the input features, would get a RSquare score of 0.0.
  
 1. Linear Regression: 0.73
 2. Decision Tree regression: 0.77 (This model overfits data)
 3. Random Forest Regression: 0.88
   

The best model which I got for this dataset with the lowest Mean Squared error and Rsquare nearest to 1 is Random Forest regression.

