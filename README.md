
Link to the sample Dashboard: https://docs.google.com/presentation/d/12_8A4pYGRNB-9pPr1TDLrR-mtxitNueUULPjYNkARqo/edit?usp=sharing

Updated 6/15/2020: add more notes and annotations for the slides

Link to the Presentation: https://docs.google.com/presentation/d/10sOgF4KqUnMWf4oruxI0mastjCT07H96pQdgFnJR6P4/edit#slide=id.g88d4106874_0_14 
 
# Machine Learning Model:

**Model Type:**
Supervised machine learning - Linear Regression (Forecasting using LSTM, Arima, XGBoost)

**Why we are using this model:**
To predict Walmart sales for 45 stores in aggreate utilizing features like temperature, holiday, CPI, fuel price and unemployment data

**How are we training our model:**
We use linear regression to fit the data set, scale and transform the data to predict sales data. After that, we compare the test data actual with the predicted value. 

**What is the model's accuracy?**
Currently, accuracy of the linear regression is 14%. Next week, we'll be using LSTM, Arima, XGBoost to increase the accuracy score.

**How does this model work?**
We will use 3 metrics to compare the effectiveness of machine learning model. The 3 metrics are: RMSE, MAE, and R-square score. 
     
     RMSE- The square root of the average of squared differences between the predicted values and actual values
     
     MAE- The average of the absolute differences between the predicted values and actual vales, all differences have the same weight
     
     R-squared score- A measure of best fit that shows how much variation of a dependent variable is explained by the independent     variable 

Source: https://github.com/Franceskling/final_project/blob/machine_learning/machine_learning/machine_learning_Models.ipynb

