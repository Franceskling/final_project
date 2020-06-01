# final_project
Group 00 Final Project
 



## Presentation

**Selected topic**

Predicting the sales with Walmart Data

**Question we hope to answer**

Can a supervised machine learning model predict unforseen sales for the business?

**Reason why we selected this topic**

Many businesses are facing a challenge due to the uncertain demands and runs out of stock sometimes, which make both the suppliers and customers upset, the store couldn't sell their products and the people do not want to buy such waste things. An automatic prediction will not only help the businesses gain more profits but also the customers to buy products that satisfies them.  

Our purpose is to ultilize supervised machine learning model and neural network to predict the sales accurately. 

**Background:**

Walmart runs several promotional markdown events through the year. These markdowns precede prominent holidays, the four largest of all,
which are the Super Bowl, Labour Day, Thanksgiving, and Christmas. The weeks including thse holidays are weighted five times higher in the evaluation than non-holiday weeks. Historical sales data for Walmart stores located in different regions are available.

If we are successful, we should be able to apply our model to predict overall sales for 45 Walmart stores in aggreate.

**Description of data source:**
This is the historical weekly sales data for 45 Walmart stores in aggreate from period 2010-02-05 to 2012-11-01.

In total, there are 8 different fields, which is listed below:
1. Store - the store number
2. Date - the week of sales
3. Weekly_Sales - sales for the given store
4. Holiday_Flag - whether the week is a special holiday week: 1 - Holiday week; 0 - Non-Holiday week
5. Temprature - Temperature on the day of sale
6. Fuel_Price - Cost of fuel in the region
7. CPI - Prevailing consumer price index
8. Unemployment - Prevailing unemployment rate

Link to source: https://www.kaggle.com/aditya6196/retail-analysis-with-walmart-data
## Git hub

# Project Team and Role Responsibilities (First Segment)

Archana Rohilla - Machine Learning, Import data from RDS DB Walmart sales into Jupyter notebook

Vick Anand - ETL analysis, build schema utilizing ERD QuickDB, Postgress and connection to AWS RDS DB

Tri Luu - Presentation and communication plan (readme.md)

Frances Klingenberger - created github master branch and tracked communications 

# Process Overview and Technology used
![alt text](https://github.com/Franceskling/final_project/blob/master/ProcessFlow.png)


![alt text](https://github.com/Franceskling/final_project/blob/master/Communication%20Plan.png)



## ETL

**Extract:** Extracted csv file from Kaggle.com 

**Transform:** We created an ETL function to revise and clean columns

**Load:** Loaded data into Postgress from Jupyter Notebook

Source: https://github.com/Franceskling/final_project/blob/ETL_Analysis/Walmart_Wkly_Sales_ETL.ipynb

## Machine Learning Model:

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

