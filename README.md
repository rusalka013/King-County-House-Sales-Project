# Microsoft Movie Analysis

**Authors:** Elena Burlando

## Overview

The objective of this project is to analyze movie data to provide insights on movie types that have performed best in the past decade. 

As an outcome of this analysis we are hoping to get: 
* Releases: 
  * Top 10 most produced genres during 2010-2020 (by entry count).
  * Top 2 most produced genres for each year (by entry count).
* Popularity: 
  * Top 10 most popular movies and genres during 2010-2019 (by number of votes). 
* Rating:
  * Top 10 highest rated genres during 2010-2019.
  * Top 10 highest rated movies during 2010-2019. 
  * Correlation between ratings and number of votes. 
* Gross Income and ROI:
  * Movies/genres with the highest domestic gross income. 
  * Movies/genres with the highest foreign gross income.
  * Movies/genres with the highest worldwide gross income. 
  * Correlation between domestic and foreign gross income.
  * Correlation between production budget and ROI. 
  * Movies/genres with the highest ROI (return on investment). 

## Business Problem

Microsoft following the success of other big tech companies is considering setting up a movie studio. This project is aiming to provide valuable information to the head of Microsoft's new movie department in the areas of movies, genres, and ROI. 

One of the main business pain points related to this project is lack of experince in the movie industry and using 
data from other sources since it doesn't have any of its own. I picked the questions above as I think the answers to those would be the most beneficial when starting from scratch. They will provide high level overview of the industry and trends. 

## Data Understanding and Methods

For this project we will be using data from: 
* [IMDB](https://www.imdb.com/)
* [Box Office Mojo](https://www.boxofficemojo.com/)
* [The Numbers](https://www.the-numbers.com/)

Variables included: movie titles, release year, genres, runtime minutes, ratings, number of votes, and gross income (domestic and foreign) made of movies from 2010 through 2020.

* Using these sources we would be able to answer our questions listed above. 
* The target variables are the top performing movie titles and genres. 
* We used descriptive analitics, averages(mean), max, and Pearson correlation to answer questions in these four categories outlined in the Overview section. 


## Data

* Over 140K data entries for movie titles, genres, and release dates from 2010-2020. 
* Over 72K data entries for average ratings and number of votes. 
* Over 1,525 & 2,636 data entries for movie budgets, domestic/foreign/worldwide gross from two datasets.


## Exploratory Findings

### RELEASES

![alt text](https://github.com/rusalka013/microsoft-movie-analysis/blob/main/Images/Top%2010%20by%20Release.png)

For this analysis we used data of over 140,734 movies.  
Documentary and Drama have been the most released movie genres in the past decade. 

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

There is little positive correlation (0.16) between rating and population indicating that these two variables have to be considered independently as we did.

There is a strong positive correlation between Domestic and Foreign Gross resulting in 47% and 53% of worldwide gross respectively. Based on two datasets, the correlation is between 0.76-0.83.

There is also a positive correlation between Production Budget and ROI: 0.58 indicating that investing into a quality production will result in higher return.

After analizing outcomes in categories: Popularity and Gross Income and ROI, we do see popsitive correlation between most popular and highest in gross and ROI genres: Animation, Adventure, Sci-Fi.  

Business Recommendations:

* Genre: Produce movies in genres: Animation, Adventure, & Sci-Fi. They are not only the most profitable genres, but also ranking highest in popularity.
* Production Budget and ROI: Invest into a quality production as it leads to higher returns.
* Gross: Release a movie in both domestic and foreign markets to get the maximum gross. Foreign gross is responsible for over half of worldwide income (~53%). 

Next Steps: 
* To analyze the trends in genres over the years. 
* To get more recent data through APIs to see how pandemic has shaped a movie industry. 
* To perform more in-depth analysis on ROI per genre. 
* To look into a cast and directors whose movies are the most popular and profitable. 



