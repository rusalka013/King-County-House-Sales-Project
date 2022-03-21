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

* Over 21K data entries of house sales with details on house and lot specs, price, date sold, and whether a house has views and has been renovated. 

## Results

### Price based on condition
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Release.png)

Price change based on condition in comparison to Average:
* -13.8% Fair
* +6.7% Good
* +16% Very Good!
 

## POPULARITY
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Popularity_mean.png)

For this analysis we used data of 72,480 movies.  
Adventure, Sci-Fi, Action, and Fantasy have been the most popular movie genres in the past decade. 

## RATING 
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Rating%20over%20100%20votes.png)

For this analysis we used data of 28,506 movies with over 100 votes. 
News, Documentary, and Biography have been the highest rated movie genres in the past decade. Their average rating is 7.1 , 7, and 6.9 respectively. 

## CORRELATION BETWEEN RATING AND POPULARITY
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Correlation%20bw%20Rating%20and%20Popularity.png)

There is a little positive correlation (0.16) between rating and population indicating that these two variables have to be considered independently. 

## DOMESTIC GROSS
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Domestic%20Gross.png)

Animation, Adventure, and Sci-Fi are performing best financially in domestic market with at or over $100M gross.  

## FOREIGN GROSS
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Foreign%20Gross.png)

Animation, Adventure, Sci-Fi are performing best financially with over $150M foreign gross. 

## WORLDWIDE GROSS
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Worldwide%20Gross.png)
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Worldwide%20Gross_2nd%20dataset.png)

For this analysis we used data two datasets: Box Office Mojo and The Numbers.  We are getting very similar results per genre. This is an indication that the outcome is correct. 
Animation, Adventure, and Sci-Fi are the top three genres with over $250M worldwide gross.  

## ROI
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20ROI.png)

Animation, Adventure, Sci-Fi are the most profitable genres. On average each of these  genres is responsible for around $200M in ROI. 

## CORRELATION BETWEEN DOMESTIC AND FOREIGN GROSS 
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Correlation%20bw%20Domestic%20and%20Foreign%20Gross.png)
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Correlation%20bw%20Domestic%20and%20Foreign%20Gross_2nd%20dataset.png)

After analyzing two dataset with financial data: The Numbers and  Box Office Mojo, 
we  discovered that there is a strong positive correlation between domestic and foreign gross.
Domestic gross is responsible  for 47%  of worldwide gross when Foreign gross is responsible for 53%.  

## CORRELATION BETWEEN PRODUCTION BUDGET AND ROI
![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Correlation%20bw%20Production%20Budget%20and%20ROI.png)

Positive correlation between Production Budget and ROI of 0.58 suggests that investing into a quality production will lead to a higher Return on Investment. 

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




