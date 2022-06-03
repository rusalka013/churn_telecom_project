# Churn Telecom Project

**Authors:** Elena Burlando

## Overview

The objective of this project is to analize Telecom Customer data in order to gain insights on what is contributing to customer churn.

As an outcome of this analysis we are aiming to get:

* factors contributing to customer churn
* reccommendations on preventive measures to reduce customers leaving


## Business Problem

Telecom company is experiencing 14.5% churn of its customers. As it is costly to the company to lose every seventh of its clients and it is also costly to acquire new clients. It is important to identify why customers are leaving to come up with preventive measures.

One of the main pain points for this project is the lack of industry/business knowledge.


## Data Understanding and Methods

For this project we will be using data from: 
* [Telecom Churn Data](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset)


Predictors: 'state', 'account length', 'area code', 'phone number', 'international plan', 'voice mail plan', 'number vmail messages', 'total day minutes', 'total day calls', 'total day charge', 'total eve minutes', 'total eve calls', 'total eve charge', 'total night minutes', 'total night calls', 'total night charge', 'total intl minutes', 'total intl calls', 'total intl charge', 'customer service calls'

* The target variable is churn.
* The main score is f1.
* We intend to use Classifiers such as Decision Tree, Random Forest, and Logistic Regression to calculate formula to predict whether a customer will churn.
* For hyper parameter tuning we will use GridSearchCV and RandomSearchCV.
* We will be following CRISP-DM process for this project.


## Data

The dataset has 21 columns (including the target column) and 3333 rows of data entries.

## Features contributing to model output:

* Total charges
* Customer service calls
* International plan 
* Total international calls
* Voice mail plan
* Number vmail messages

![alt text](https://github.com/rusalka013/churn_telecom_project/blob/main/Visuals/Absolute_Feature_Average_Impact.png)




## Results

### Price based on sqft living
![alt text](https://github.com/rusalka013/King-County-House-Sales-Project/blob/main/Visuals/Correlation%20bw%20sqft_living%20and%20Price.png)

For every 2/100 percent increase in square feet there is one percent increase in price.


### Price based on condition
![alt text](https://github.com/rusalka013/King-County-House-Sales-Project/blob/main/Visuals/Price%20vs%20Condition.png)

Price change based on condition in comparison to Average:
* -13.8% Fair
* +6.7% Good
* +16% Very Good!
 

## Price based on grade
![alt text](https://github.com/rusalka013/King-County-House-Sales-Project/blob/main/Visuals/Price%20vs%20Grade.png)

Price change based on a grade in comparison to Very Good:
* +6.6% Excellent 
* -7% Better
* -22.7% Good
* -38% Average
* -56.7% Low Average
* -64.4% Fair
 

## Price based on month: 
![alt text](https://github.com/rusalka013/King-County-House-Sales-Project/blob/main/Visuals/Price%20vs%20Month.png)

Price change based on a month in comparison to January:
* +4.2% March
* +6.1% April
* +7.8% May
* +9.5% June
* +8.5% July
* +8% August
* +8.3% September
* +9% October
* +8.2% November
* +7.9% December
 

## Price based on city:
![alt text](https://github.com/rusalka013/King-County-House-Sales-Project/blob/main/Visuals/Price%20vs%20City.png)

Price change based on a city in comparison to Auburn:
* +64.1% Bellevue
* +42.3% Bothell
* +35.2% Duvall
* +9.7% Enumclaw
* +53.7% Issaquah
* +5.1% Kent
* +63.5% Kirkland
* +17.8% Maple Valley
* +85.8% Mercer Island
* +36.5% North Bend
* +58.2% Redmond
* +24.5% Renton
* +64.7% Seattle
* +46.8% Shoreline
* +42.2% Snoqualmie
* +18.2% Tukwila
* +48.2% Woodinville
* +108.6 Yarrow Point


## Conclusions

Business Recommendations for customers (sellers): 

* condition: 
Perform maintenance and upgrades to increase price by up to 16% (from Average to Very Good).   

* grade: 
Renovate a house to increase the price by up to 71% (ex.renovating a house from Fair to Very Good grade will increase the value by 64%). However, additional calculaltions on ROI has to be done prior to this suggestion.  

* month: 
Sell a house in summer to early fall months for up to 9.5% higher in price. Best months to sell are June and October.  
 
* city: 
Houses in cities south of Seattle sell for at least 20% lower compare to houses West and North. 

Next Steps:  
* To acquire additional feature information (such as staged or not staged, fixture updates, curb appeal, color of interior and exterior walls, etc) regarding houses sold. Adding these features to our model can further expand agent's knowledge on what suggestions to make to clients that could increase the house value. 
* To get more recent house data through APIs (redfin API) to understand Housing Market trends in the past 20 years.   




