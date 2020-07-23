---
title: "Part II: REGRESSION ANALYSIS"
author_profile: false
collection: casestudies
---

## CH07A Finding a good deal among hotels with simple regression
Vienna, Austria is a popular tourist destination for business and leisure. With the `hotels-vienna` dataset, we search for a good deal for a single night in November 2017 among 3-4 star hotels located in the center of Vienna. We use regression analysis to find what the hotel price “should be" for various levels of distance to the city center. Then we compare that price to the actual price of each hotel to identify the especially low values. First, we use bin scatters and a lowess non-parametric regression and see that hotels further away from the city center are, on average, less expensive. In order to find out by how much (on average), we apply linear regression. We find that hotels that are 1 mile further away from the city center are, on average, 14 dollars cheaper in our data. After examining the residuals of the linear regression of hotel prices on distance to the city, we find the five most underpriced hotels. However, we also see that simple linear regression with distance to the city center explains 16% of the overall variation in hotels prices hence this may not produce the best possible prediction.

This case study introduces non-parametric regression such as lowess, and linear regression (OLS), residuals and goodness of fit (R-squared).


## CH08A Finding a good deal among hotels with non-linear function
Vienna, Austria is a popular tourist destination for business and leisure. With the `hotels-vienna` dataset, we search for a good deal for a single night in November 2017 among 3-4 star hotels located in the center of Vienna. In order to capture the non-linear pattern between distance and hotel price, we measure relative price differences. We examine four regressions and pick the log-level that shows that hotels that are 1 mile farther away from the city center are 13% less expensive, on average.

This case study illustrates the use of logarithms in linear regression and the transformation of variables, and the coefficient interpretations in different setups. It allows instructors to demonstrate how the focus of interest of the data analysis can affect the choice of applied methods.


## CH08B How is life expectancy related to the average income of a country?
In wealthier countries people generally live longer. Can we find countries where people live longer than what we would expect based on their average income? We use the `worldbank-lifeexpectancy` data based on the WDI database, and examine data from a single year, 2017 for 182 countries. We search for a regression model (functional form) that captures the shape and strength of the association. With our preferred model, we find a few countries where people live more than seven years longer than what we could expect given the countries’ GDP per capita.

This case study illustrates the transformations of variables (logs, per capita measures, weights) and non-linear functional forms (spline, polynomial). It shows how to visualize regressions with variables in logs.


## CH08C Measurement error in hotel ratings
What can we do about measurement error during data analysis? With the hotels-vienna dataset, we search for a good deal among hotels in Vienna, Austria. We examine hotel ratings published on a price comparison website. Ratings vary between 1 and 5, 5 being excellent and the website shows the average value of ratings for each hotel. We try to uncover an association between price and quality by a regression of hotel price on customer rating for two cases: when the average rating is based on a few and when it is based on many ratings. We find that there is a substantial measurement error in average customer ratings among hotels where that average rating is based on a few customers’ reports.

This case study illustrates the effect of classical measurement error.

## CH09A Understanding gender and age differences in earnings
Do women working as market analyst earn the same as men (called the gender gap)? And does the answer to this question depend on the age of the employee? Using the `cps-morg` data, based on the Current Population Survey (CPS) of the U.S. in 2014, we focus on the occupation category called "Market research analysts and marketing specialists". We examine the pattern of association between log earnings and gender first and then extend the analysis by looking at the gender gap by age. We find a non-linear pattern: the gender gap varies by age. We discuss to what extent this result may be generalized to a larger population.

This case study shows illustrates the use of **CI** and **SE** of regression coefficients. It also shows how to **test hypotheses about regression coefficients**. It allows instructors to demonstrate **presentation** of regression results.


## CH09B How stable is the hotel price–distance to center relationship?
European historic cities are popular tourist destinations. We have seen the nature of relationship between price and distance in Vienna. Will the hotel price-distance pattern change if we look at other European cities or for another date? Using the `hotels-europe` data, we look at 3-4 star hotels in Vienna and compare prices for four different dates. We then look at hotel prices in Amsterdam and Barcelona for the same weekday in November 2017. Finally, we examine whether we find a similar price-distance pattern in Vienna for another type of accommodation. We conclude that external validity across dates and accommodation types seems solid, but across space seems moderate.  

This case study illustrates the **potential issues with external validity** and how we to think about it in a real life setting.


## CH10A Understanding the gender difference in earnings
Is it true that female employees with a graduate degree earn less than men on average (called the gender gap)? We look at data from the Current Population Survey (CPS) of the U.S. in 2014 and use the `cps-earnings` dataset. We narrow our focus to people with graduate degree, aged 24 to 65, who reported working at least 20 hours a week. We examine the pattern of association between log earnings, gender and age by multiple regressions. We also run multiple regressions to investigate earnings’ differences by three categories of educational degree: master’s, professional and PhD. We examine interactions as we consider whether the patterns with age are similar or different for men versus women. We find that gender differences, whether due to discrimination or productivity differences, tend to be small among younger employees and large among middle-aged employees.  

This case study illustrates how to **estimate multiple linear regressions** and how to **interpret and generalize** their results. It shows how to **visualize different patterns of association**, including non-linear patterns between different groups. It allows instructors to demonstrate the difficulty of drawing causal conclusions from regression estimates using cross-sectional data.


## CH10B Finding a good deal among hotels with multiple regression
Vienna, Austria is a popular tourist destination for business and leisure. With the `hotels-vienna` dataset, we search for a good deal for a single night in November 2017 among 3-4 star hotels located in the center of Vienna. We define good deal as a hotel that is inexpensive relative to its quality and distance to the city center. We measure quality by stars (3,3.5 and 4) and average customer rating (ranging from 2 to 5). We run multiple regressions and then focus on the difference of actual (log) price from its predicted value. After finding the five hotels with the largest residuals from the regression, we produce a short-list that shows the least expensive hotels relative to their distance to the city center and their quality.  

This case study illustrates the use of **multiple regressions** in **prediction** and **residual analysis**.


## CH11A Does smoking pose a health risk?
Are smokers less likely to remain healthy than non-smokers? We use the `share-health` data from the SHARE survey (Survey for Health, Aging and Retirement in Europe). *(SHARE is a longitudinal survey studying the process of aging on a large sample of individuals across many European countries. It has interviewed the same individuals every two years since 2004.)* We focus on people who were 50 to 60 years old and said to be in good health in 2011. We look at how they rated their health in 2015 and see who changed their answer to not healthy. First, we estimate a linear probability model (LPM) with being healthy in 2015 as the binary dependent variable and whether the individual is a current smoker in 2011 as the only explanatory variable. Then we condition on various quantitative and qualitative variables and estimate LPM, logit and probit models for the probability of staying healthy. We find that 50 to 60 year-old healthy smokers are 10% less likely to stay healthy than non-smokers of the same gender, age, education, income, and body weight, whether they exercise or not.

This case study illustrates the use of the **linear probability model**, the **logit**, and the **probit**. It allows instructors to demonstrate various **measures of fit** for **probability predictions (R-squared, Brier score)**.


## CH11B Are Australian weather forecasts well-calibrated?
## CHECK under Figure 11.6 it says 2005/6 but in text 2015/16
Should we take an umbrella when the Australian weather forecast predicts rain? We use the `NAME OF DATA` data covering 350 days in 2015/16 and look at rain forecast and actual rain for the Northern Australian city of Darwin. We consider predictions of rain for the day following the prediction. *(The predictions come as probabilities such as 0%, 10% or 20% chance of rain tomorrow, hence we can evaluate how well-calibrated they are.)* We define a rainy day as a day with at least 1mm rain and form a binary variable to capture whether it actually rained that day. We find that the prediction of rain in Australia is well-calibrated.  

This case study illustrates the **use of calibration**.

## CH12A Returns on a company stock and market returns
How do monthly returns on a company stock move together with monthly market returns? We choose the Microsoft stock and the S&P 500 stock market index (S&P 500) that is a weighted average of 500 company stock prices listed on the New York Stock Exchange and Nasdaq. Using the `NAME OF DATA` dataset, we have daily data on the closing price of the Microsoft stock and the S&P 500 for 21 years. We define monthly time series of prices as the closing price on the last day of each month and monthly returns as the percent changes of prices between the last days of each month. After estimating a simple regression, we find that returns on the Microsoft stock tend to be larger than average by 1.26% in the months when returns on the S&P 500 are larger than average by 1%.

This case study illustrates **simple time series regression** with relative changes as variables. It allows instructors to demonstrate **visualization** of **time series regression**.


## CH12B Electricity consumption and temperature
How does residential electricity consumption relate to temperature? We examine monthly electricity consumption data from Arizona state and monthly temperature data from one weather station in Phoenix. Covering 17 years, we use the `arizona-electricity` dataset that transforms the weather data to "cooling degree days" and "heating degree days" per month. These measure the number of days in a month when most residents would use electricity for cooling or heating. We estimate time series regressions in changes and with and without season dummies. We find that temperature is strongly related to residential electricity consumption in Arizona and there is a strong seasonality.

This case study illustrates how to handle and interpret **seasonality** and **lagged associations**, and how to **estimate robust standard errors** in time series regressions.
