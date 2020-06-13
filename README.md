
Link to the sample Dashboard: https://docs.google.com/presentation/d/12_8A4pYGRNB-9pPr1TDLrR-mtxitNueUULPjYNkARqo/edit?usp=sharing
 

## Project Outline

# Project Team and Role Responsibilities (First Segment)

Archana Rohilla - Machine Learning, Import data from RDS DB Walmart sales into Jupyter notebook

Vick Anand - ETL analysis, build schema utilizing ERD QuickDB, Postgress and connection to AWS RDS DB

Tri Luu - Presentation and communication plan (readme.md)

Frances Klingenberger - created github master branch and tracked communications 

# Project Team and Role Responsibilities (Second Segment)

Archana Rohilla - Expanded Machine Learning Model

Vick Anand - Created Dashboard with Tri

Tri Luu - Created Dashboard with Vick 

Frances Klingenberger - Manage Github and expanded Presentation 

# Project Team and Role Responsibilities (Third Segment)

Archana Rohilla - Machine Learning 

Vick Anand - Created Dashboard with Tri, worked on Machine Learning with Archana

Tri Luu - Created Dashboard with Vick 

Frances Klingenberger - GitHub and Presentation

# Process Overview and Technology used
![alt text](https://github.com/Franceskling/final_project/blob/master/ProcessFlow.png)






## ETL

**Extract:** Extracted csv file from Kaggle.com 

**Transform:** We created an ETL function to revise and clean columns

**Load:** Loaded data into Postgress from Jupyter Notebook

Source: https://github.com/Franceskling/final_project/blob/ETL_Analysis/Walmart_Wkly_Sales_ETL.ipynb

## Machine Learning Model:

*See full explaination of ML described in Jupyter Notebook file 

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

Source: https://github.com/Franceskling/final_project/blob/machine_learning/machine_learning/machine_learning_4.ipynb

## Database
Develop database schema utilizing ERD DB below:

Sources: https://github.com/Franceskling/final_project/blob/ETL_Analysis/QuickDBD-WMT_Weekly_Sales.sql

RDS DB endpoint: walmartsales.ctixdh2hiprk.us-east-2.rds.amazonaws.com

![alt text](https://github.com/Franceskling/final_project/blob/master/databsae_QBD.PNG)

