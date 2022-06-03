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


## Insights from Global Importance of SHAP values:

* High 'Total_charges' have a high positive impact on model.
* Customer service calls have positive moderate to high impact.
* Having international plan have positive low to high impact.
* Low # of intl calls has positive moderate impact on model.
* High total of intl minutes has positive medium impact.
* High number of voice messages has low to moderate negative impact.
* Having voice mail plan has negative low moderate effect.

![alt text](https://github.com/rusalka013/churn_telecom_project/blob/main/Visuals/global_importance_of_each_feature_violin.png)


## Results

### Total charges impact on churn

High charges lead to high probability of customer churn. 

![alt text](https://github.com/rusalka013/churn_telecom_project/blob/main/Visuals/Relationships%20between%20Total_charges%20and%20churn.png)


### Customer service calls impact on churn

4+ customer service calls lead to moderate to high likelihood of churn regardless if total charges are low or high. 

![alt text](https://github.com/rusalka013/churn_telecom_project/blob/main/Visuals/Relationships_between_customer%20service%20calls_and_churn.png)
 

## International plan impact on churn

Customers with current international plans and low international calls are more likely to churn.

![alt text](https://github.com/rusalka013/churn_telecom_project/blob/main/Visuals/Relationships_between_international%20plan_and_churn.png)

 

## Voice mail plan impact on churn 

Clients without voice mail plan are 10% more likely to churn vs those with one.

![alt text](https://github.com/rusalka013/churn_telecom_project/blob/main/Visuals/Relationships_between_voice%20mail%20plan_and_churn.png)


## Conclusions

Business Recommendations: 

* total charges: 
Offer package plans for users with high usage. On a current plan high usage leads to high charges which are highly correlated with churn.

* customer service calls: 
Improve customer service call experience by looking closely into customer service call support to gain a more granular understanding on what is driving customers to churn. 2+ customer service calls lead to moderate to high likelihood of churn regardless of total charges.

* voice mail: 
Offer voice mail plan. Clients without voice mail plan are 10% more likely to churn vs those with one.

* international plan: 
Offer different international plans based on usage: low, medium, high. Customers with current international plans and low international calls are more likely to churn.

Next Steps:  
* To gain a better understanding of the Telecom plans through business stakeholders.
* Obtain more break down data on customer service calls such as waiting time, whether a customer issue has been resolved, what are the issues that customers called for, etc.
* To compare Telecom's pricing structure and plans with competitors.



