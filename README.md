
Link to Presentation/Dashboard: https://public.tableau.com/shared/NBPGWZXQT?:display_count=y&:origin=viz_share_link

 

# Project Outline

## Background

Our project focuses on sales forecasting and how certain outside influences can affect store performance. We will predict sales for Walmart based on three years of data across 45 stores by using various machine learning models. We want to determine which model generates the most accurate predictions. 

## Project Team and Role Responsibilities (First Segment)

Archana Rohilla - Created preliminary Machine Learning Model, Imported data from RDS Database "Walmart sales" into Jupyter Notebook 

Vick Anand - ETL analysis, build schema utilizing ERD QuickDB, Postgress and connection to AWS RDS DB

Tri Luu - Presentation and communication plan (readme.md)

Frances Klingenberger - created github master branch and tracked communications 

## Project Team and Role Responsibilities (Second Segment)

Archana Rohilla - Imported data from RDS Database "Walmart sales" into Jupyter notebook, Expanded Machine Learning Model

Vick Anand - Created Dashboard with Tri

Tri Luu - Created Dashboard with Vick 

Frances Klingenberger - Manage Github and expanded Presentation 

## Project Team and Role Responsibilities (Third Segment)

Archana Rohilla - Expanded Machine Learning Model

Vick Anand - Created Dashboard with Tri and worked on Machine Learning Model with Archana

Tri Luu - Created Dashboard with Vick 

Frances Klingenberger - Manage Github and expanded Presentation 

## Project Team and Role Responsibilities (Third Segment)

Archana Rohilla - Finalized Machine Learning Model, Practiced Presentation

Vick Anand - Finalized Dashboard and Machine Leanring Model, Practiced Presentation

Tri Luu - Finalized Dashboard and Presentation, Practiced Presentation

Frances Klingenberger - Manage Github and Finalized Presenatation, Practiced Presentation

# Process Overview and Technology used
![alt text](JPGS/ProcessFlow.png)






# ETL

**Extract:** Extracted csv file from Kaggle.com 

**Transform:** We created an ETL function to revise and clean columns

**Load:** Loaded data into Postgress from Jupyter Notebook

Source: ETL/Walmart_Wkly_Sales_ETL.ipynb

# Machine Learning Model:

*See full Machine Learning code and further description in Jupyter Notebook file for the calculated metrics (RMSE, MAE, R-square score)

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

# Database
Develop database schema utilizing ERD DB below:

Sources: ETL/QuickDBD-WMT_Weekly_Sales.sql

Database Connections & Steps: database/Steps for Database & Connections.docx

RDS DB endpoint: walmartsales.ctixdh2hiprk.us-east-2.rds.amazonaws.com

![alt text](https://github.com/Franceskling/final_project/blob/master/JPGS/databsae_QBD.PNG)

# Dashboard

Storyboard sample:

![alt_text](https://github.com/Franceskling/final_project/blob/master/Resources/Dashboard.png)



