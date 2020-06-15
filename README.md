
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
The data was imported from the RDS database of the AWS.
Link to the machine learning code: https://github.com/Franceskling/final_project/blob/machine_learning/machine_learning/machine_learning_Models.ipynb

# Data Preprocessing:
- The cleaned data was then divided into the input(X) and the target/output(y) features. Also, the non-relevant columns were dropped from the data.
  All the columns to be used in the model must contain a numerical data type.

- The data needs to be split into the training and testing data-sets before fitting in the StandardScaler instance. This prevents testing data from 
  influencing the standardization function.

- Scale the Data:Feature Scaling is a technique to standardize the independent features present in the data in a fixed range. It is performed during the data 
  pre-processing to handle highly varying magnitudes or values or units. If feature scaling is not done, then a machine learning algorithm tends 
  to weigh greater values, higher and consider smaller values as the lower values, regardless of the unit of the values.

# Performance Metrics:

# Root Mean Squared Error:
Root Mean Square Error (RMSE) is the standard deviation of the residuals (prediction errors). Residuals are a measure of how far from the regression line 
data points are; RMSE is a measure of how spread out these residuals are. In other words, it tells you how concentrated the data is around the line of best fit.

# Mean Absolute Error:
In statistics, mean absolute error (MAE) is a measure of errors between paired observations expressing the same phenomenon.

# R-squared:
R-squared (R2) is a statistical measure that represents the proportion of the variance for a dependent variable that's explained by an independent variable or 
variables in a regression model. R-squared is always between 0 and 100%:
- 0% indicates that the model explains none of the variability of the response data around its mean.
- 100% indicates that the model explains all the variability of the response data around its mean.

# Linear Regression Model:
Linear regression is a statistical model that is used to predict a continuous dependent variable based on one or more independent variables fitted to the 
equation of a line. Multiple linear regression builds a linear regression model with two or more independent variables. In this case, 
the dependent variable(target variable i.e. y) is dependent upon several independent variables(X). A regression model involving multiple variables can be 
represented as:
y = b0 + m1b1 + m2b2 + m3b3 + … … mnbn
This is the equation of a hyperplane.

- Results: Root Mean Squared Error=529802.0649517294, Mean Absolute Error=440285.20259857585, R-squared=0.1447931750333451
- Since R-squared is only 14%, it means that this Linear Regression Model is not good in prediction and needs some improvement.

This Linear Regression Model can be improved by using the "lag". A "lag" is a fixed amount of passing time; One set of observations in a time series 
is plotted (lagged) against a second, later set of data. The kth lag is the time period that happened “k” time points before time i. The "lag" has been 
implemented in Store-1 data. 

# Linear Regression Model using "lag":
The link to the file is: https://github.com/Franceskling/final_project/blob/machine_learning/machine_learning/sales_forecast_store1.ipynb

- Results: 
Mean Absolute Error: 29271.61936361866
Mean Squared Error: 1494186688.7343
Root Mean Squared Error: 38654.711080724686
The value of root mean squared error is 38654.71, which is slightly greater than 2% of the mean value which is 1.561364e+06. 
This means that this algorithm is accurate and can make reasonably good predictions.

# Random Forest Regressor Model:
A random forest is an ensemble model that consists of many decision trees. Predictions are made by averaging the predictions of each decision tree.
- Results: Root Mean Squared Error=118809.7423062449, Mean Absolute Error=65539.96687047854, R-squared=0.9569921262077471

- Since R-squared is 95%, it means that this Random Forest Regression Model is good in prediction as compared to the Linear Regression Model.

# Data Transformation:
The predicted data is exported or saved into a simpler format for storage and future use, such as a CSV, spreadsheet, or database file.




