
Link to the sample Dashboard: https://docs.google.com/presentation/d/12_8A4pYGRNB-9pPr1TDLrR-mtxitNueUULPjYNkARqo/edit?usp=sharing

Updated 6/15/2020: add more notes and annotations for the slides

Link to the Presentation: https://docs.google.com/presentation/d/10sOgF4KqUnMWf4oruxI0mastjCT07H96pQdgFnJR6P4/edit#slide=id.g88d4106874_0_14 
 
# Data Selection:
The data was taken from Kaggle. The link to source is: https://www.kaggle.com/aditya6196/retail-analysis-with-walmart-data

# Data Cleaning:
The data was cleaned using an ETL function which was described in the Walmart_Wkly_Sales_ETL.ipynb file of the ETL_Analysis branch. The cleaned 
data was then stored in the postgres as 'Weekly_Sales', 'Features' and 'Holidays' tables. The data was then stored in the RDS database of the
Amazon Web Services(AWS) so that it can be easily imported to some other remote file. 

# Importing the Data in the jupyter notebook:
Here, the data was imported from the RDS database of the AWS.

# Data Preprocessing:
- The cleaned data was then divided into the input(X) and the target/output(y) features. Also, the non-relevant columns were dropped from the data.
  All the columns to be used in the model must contain a numerical data type.

- The data needs to be split into the training and testing data-sets before fitting in the StandardScaler instance. This prevents testing data from 
  influencing the standardization function.

- Scale the Data:Feature Scaling is a technique to standardize the independent features present in the data in a fixed range. It is performed during the data 
  pre-processing to handle highly varying magnitudes or values or units. If feature scaling is not done, then a machine learning algorithm tends 
  to weigh greater values, higher and consider smaller values as the lower values, regardless of the unit of the values.

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

