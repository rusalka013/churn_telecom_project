# King County House Sales Project

**Authors:** Elena Burlando

## Overview

The objective of this project is to analyze housing data for King County to provide insights on variables that effect sale price and also determine if there any pricing trends that can project future growth of certain markets. 

As an outcome of this analysis we are hoping to get: 

Insights for real estate agents: 
 * Price drivers (predictors)
 * Housing market trends based on city

## Business Problem

A local real estate agency in King County WA is looking to develop a web tool that would help clients to estimate the sale prices for their homes. This tool will be used as a marketing tool to engage and acquire new customers. Ideally, we would like to include variables that sellers can control such as staging, curb appeal, remodeling, fixture updates, the color of walls, etc. This will provide visibility to sellers on what investments can contribute to the price increase of their house.

In addition, the agency is looking to develop an internal tool that would showcase current Housing Market trends. This tool will help their real estate agents to reach potential house sellers ahead of the competition and help their buying clients to get a better return on the investment.

One of the main business pain points is high competition from large established and small real estate agencies in the area. Proposed tools will differentiate the agency from the competition and lead to higher engagement and sales.


## Data Understanding and Methods

For this project we will be using data from: 
* [King county house data](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r)
* [Zipcode list](https://www.ciclt.net/sn/clt/capitolimpact/gw_ziplist.aspx?FIPS=53033)


Predictor variables: 'date', 'bedrooms', 'bathrooms', 'sqft_living', 'sqft_lot', 'floors', 'sqft_above', 'sqft_basement', 'yr_built', 'yr_renovated', 'zipcode', 'lat', 'long', 'sqft_living15', 'sqft_lot15', 'waterfront', 'view', 'grade', 'condition', 'city' for house sales between 2014 and 2015 for King County WA.

* Using these sources we would be able to answer our questions listed above. 
* The target variable is sale price.  
* We intend to use Multiple Linear Regression to calculate formula to predict future house sale price. 
* We will be following CRISP-DM process for this project. 


## Data

Over 21K data entries of house sales with details on house and lot specs, price, date sold, and whether a house has views and has been renovated. 

## Correlation between Features and Target
![alt text](https://github.com/rusalka013/King-County-House-Sales-Project/blob/main/Visuals/Price%20and%20Features%20Correlation.png)


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




