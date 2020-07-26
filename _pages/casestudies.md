---
permalink: /casestudies/
title: "Case Studies"
toc: true
author_profile: false
redirect_from:
  - /md/
  - /casestudies.html
---

{% include base_path %}

> ## *Data analysis is a process



# Data and code info
**To get code, data, graphs**, we advise to follow instructions on how to get all codes and dependencies for  [**Stata**](get-allcode-stata) or [**R**](get-allcode-R) or [**Python**](get-allcode-py). All the data may be downloaded from [Get Data](link-google-drive)


[PART 1: DATA EXPLORATION](#part-i-data-exploration)  
[PART 2: REGRESSION ANALYSIS](#part-ii-regression-analysis)  
[PART 3: PREDICTION](#part-iii-prediction)  
[PART 4: REGRESSION ANALYSIS](##part-iiii-causal-analysis)  


# PART I: DATA EXPLORATION

## CH01A Finding a good deal among hotels: data collection
Vienna, Austria is a popular tourist destination for business and leisure. From the hundreds of places that offer accommodation, we want to pick a hotel that is underpriced relative to its location and quality for a weekday in November 2017. Can we use data to help this decision? What kind of data would we need, and how could we get it?

This case study illustrates how to collect appropriate data from the web on multiple offers. It describes what we want from such data and what data source we would need. The data is collected by **web scraping**, and it results in a single **data table.** It discusses the **quality of the data** from the perspective of the question and how it is determined by the way the data was born. There is no dataset to analyze in this case study in this chapter. Subsequent case studies (2A, 3A, 7A, 8A, 9B, 10B) will use the data desctibed here to illustrate steps of data analysis that lead to ultimately answering the main question.
 
![Vienna](/images/vienna1.jpg){:height="70%" width="70%"}

## CH01B Comparing online and offline prices: data collection
Do online and offline prices of the same products tend to be the same? To answer that question, we need data on both the online and offline (in store) price of many products. Such data was collected as part of the Billion Prices Project (BPP; http://www.thebillionpricesproject.com), an umbrella of multiple projects that collect price data for various purposes using various methods.

This case study illustrates how to combine different data collection methods and what are the challenges with such data collection. It discusses how products were selected and how prices were measured, and what those methods imply for coverage of observations and reliability of variables. There is no dataset to analyze in this case study. Case study 6A will use the data described here to investigate whether online and offline prices tend to be the same.

## CH01C Management quality: data collection
How different are firms and other organizations in the terms of their management practices? Is the quality of management related to how large the firms are? Is it affected by whether the owners are the company founders or their families? To answer these, and many related, questions, we need data on management quality. Such data was collected from many organzations by the World Management Survey (WMS; https://worldmanagementsurvey.org/), an international research intitative to measure the differences in management practices across organizations and countries.

This case study illustrates how to collect data by surveys. It discusses **sampling** and its practical issues, and how to use a set of survey questions to measure and abstract concept such as the quality of management. This case study, similarly to the other case studies in this chapter, illustrates the choices and trade-offs data collection involves, practical issues that may arise during implementation, and how all that may affect data
quality. There is no dataset to analyze in this case study. Case studies 4A and 21A will use the data described here to investigate how management quality is related to firm size and how it is affected by ownership. 

## CH02A Finding a good deal among hotels: data preparation
Continuing with our search for a hotel that is underpriced relative to its location and quality in Vienna, we have scraped data from the web, and we've got a data table. But how should we start working with this data? In particular, how should we identify hotels, how should we make sure each hotel features only once in the data, and how should we select the variables we would consider for our future analysis? 

This case study illustrates how to find problems with observations and variables and uses the `hotels-vienna` dataset. It illustrates the various **types of variables**. It shows how to create a **tidy data table** and how to deal with **missing values** and **duplicates**. It allows instructors to demonstrate the importance of **data cleaning** and the common **steps of data wrangling**. We described data collection and quality in case study 01A, and we will use the data in case studies 3A, 7A, 8A, 9B, and 10B to illustrate steps of data analysis that lead to finding good deals.

**Code**: [**Stata**](link) or [**R**](link) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  

## CH02B Displaying immunization rates across countries
Immunization against measles is an effective way to prevent the disease and may save the lives of children. But how do various countries fare in terms of their immunization rate? We use the World Development Indicators data website maintained by the World Bank to look at countries’ annual immunization rate and GDP per capita.  

This case study illustrates how to store **multi-dimensional data**. It uses the `world-bank-immunization` dataset and shows a data structure focusing on two ID variables (country and year) and two other variables (immunization rate and GDP per capita). It allows instructors to demonstrate **xt panel data** tables in **long format** and **wide format**. Case study 23B will use the data described here to investigate the effect of immunization on the survival chances of children.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  

## Ch02C Identifying successful football managers
The English Premier League (EPL) is the top football (soccer) division in England. Team managers, as coaches are known in football, arguably play a ery important role in the success of their teams. Thus, we want to identify the most successful football manager in the EPL. Covering 11 years, the `football` dataset covers  all games played in the EPL and data on managers, including which team they worked at and when. We create a workfile by joining two different data tables. After defining the measure of success as average points per game, we identify the most successful managers.  

This case study introduces how to prepare data for analysis and illustrates **linking data tables** with different kinds of observations. It shows how to combine two data sources and what kinds of problems can arise while doing so. It allows instructors to demonstrate **entity resolution**, **relational data**, tidy data tables, and linking data tables. Case study 24B will use this data to uncover the effect of replacing managers of underperfoming teams on subsequent team performance.

**Code**:   [**Stata**](https://github.com/gabors-data-analysis/da_case_studies/blob/master/ch02-football-manager-success/ch02-football-manager-success.do) or [**R**](https://github.com/gabors-data-analysis/da_case_studies/blob/master/ch02-football-manager-success/ch02-football-manager-success.R) or [**Python**](clink) or  [ALL](link)  
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  

![pep-and-fergie](/images/pep-and-fergie.jpg){:height="50%" width="50%"}

 [source](https://www.soccerladuma.co.za/news/articles/international/categories/english-premier-league/sir-alex-ferguson-sends-pep-guardiola-a-warning/228353)


## Ch03A Finding a good deal among hotels: data exploration
Further continuing our search for a good deal (a hotel in Vienna that is underpriced for its location and quality), we've got a clean data table and identified the variables we want to analyze. How should we start the analysis? In particular, how should we explore the most important variables, why should we do that, and what conclusions can we draw from such exploratory analysis?

This case study uses the `hotels-vienna` dataset to illustrate how to describe the **distribution of variables** and how to use the findings to identify potential problems in the data, such as **extreme values**. The case study also illustrate how to make **decisions about extreme values**, guided by the ultimate question of the analysis. Along the way, it introduces guidelines for **data visualization** in general, and the design of **histograms** in particular. Case studies 01A and 02A describe data collection and cleaning, and we will use the data in case studies 7A, 8A, 9B, and 10B to illustrate further steps of data analysis that lead to finding good deals.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch03B Comparing hotel prices in Europe: Vienna vs London
How can we compare hotel markets over Europe and learn about characteristics of hotel prices? Can we visualize two distributions on one graph? What descriptive statistics would best describe each distribution and their differences? Can we visualize descriptive statistics?

This case study uses the `hotels-europe` dataset and selects 3-4 star hotels in Vienna and London to compare the distribution of prices for a weekday in November 2017. It illustrates the comparison of distributions and the use of histograms and density plots. It illustrates the use of some of the most important **descriptive statistics** for quantitative variables and their visualizations, **box plots** and **violin plots**.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch03C Measuring home team advantage in football
Is there such a thing as home team advantage in professional football (soccer)? That is, do teams that play in their home stadium tend to perform better? And how shoudl we measure better performance? 

This case study uses the `football` dataset, with data on the games played in the English Premier League (EPL) during the 2016/17 season. The case study shows the use of **exploratory data analysis** to answer a substantive question and introduces guidelines to present statistics in a good table.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-football).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  

## Ch03D Distributions of body height and income
Are the distributions of body heigh and family income well approximated by theoretical distributions? Answering these questions can help characterize their distributions and provide guidance for future analysis on how to use these variables.

In this very short case study, we examine survey data collected by the Health and Retirement Study in the U.S.A. in 2014 (`height-income-distributions` dataset). We show that the height of women aged 55-60 can be described by the **normal distribution**, whereas the income of their households is reasonably well characterized by the **lognormal distribution**. 

![income](/images//Ch03_figures/ch03-figure-11b-hist-income-log.png){:height="50%" width="50%"}

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch04A Management quality and firm size: describing patterns of association
Are larger companies better managed? We want to explore the association between management quality and firm size in a particular country (Mexico). Learning about this association can help benchmarking the management quality of firms of different sizes and assess potential benefits to having larger firms. To answer this question we need to define the y and x variables in this comparison. In particular, we need to assess how the variables in the dataset correspond to the abstract concepts of management quality and firm size.

This case study uses the Mexican subsample of the World Management Survey dataset (`wms-management-survey`) from 2013. It illustrates how we can measure **latent variables** by **proxy variables** in the data and uncover patterns of association betewen those variables. It illustrates the concepts of **conditional probabilities**,  **conditional distributions**, and **joint distributions**. The case study introduces informative ways to visualize various aspects of patterns of association, such as the **stacked bar chart**, the **scatterplot**, the **bin scatter**, and comparing **box plots** and **violin plots**. We have introduced the data used here in case study 01C.

![wms](/images//Ch04_figures/ch04-figure-6b-wms-mex-violin-mgmt-emp3bins.png){:height="50%" width="50%"}

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH05A What likelihood of loss to expect on a stock portfolio?
Can we find out the future likelihood of a large loss on a stock portfolio based on data from the past? We choose the S&P 500 stock market index as our investment portfolio, and we defining a large loss as an at least 5% drop in returns from one day to another. We can easily calculate the proportion of such days in the data, but we are interested in future losses not past ones. To answer our question we need to make generalizations from our data. Such generalizations are bound to bring uncertainty, and we would like to quantify that uncertainty, too.

This case study uses the `sp500` dataset that covers day-to-day returns on the S&P 500 stock market index for 11 years to illustrate how we can generalize an estimated statistic from a particular dataset to the **population**, or **general pattern**, it represents, and beyond, to the general pattern we are interested in. The case study illustrates the concept of **repeated samples**. It shows how to estimate the **standard error** by **bootstrap** or using a formula, and how to construct and interpret a **confidence interval**. It also illustrates how to think about **external validity**.

![bootsrap](/images/bootstrap.jpg){:height="30%" width="30%"}

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH06A Comparing online and offline prices: testing the difference
Do online and offline prices of the same products tend to be the same? Answering this question can help make better purchase choices, understand the business practices of retailers, and it can inform whether we can use  online data in approximating offline prices for policy analysis.

This case study uses the `billion-prices` dataset. We examine online and offline prices of retail products in the U.S. in 2015-16. The case study illustrates how to translate a more abstract question into an inquiry about a **statistic** (here the average difference). It shows how to formulate a **null hypothesis** and an **alternative hypothesis** and how to carry out a **hypothesis test** in two ways, by calculating the **t-statistic** and comparing it to an appropriate **critival value**, and by using the **p-value**. The case study also illustrates the perils of testing **multiple hypotheses** and how that may reveal artificial features of the data (here measurement error). We have introduced the data used here in case study 01B.


**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH06A Testing the likelihood of loss on a stock portfolio
When we want to learn about the likelihood of large future losses on our portfolio, we can use the confidence interval to quantify the uncertainty from estimating it from data on past returns. But we can ask a more pointed question, too: whether our stock portfolio is will suffer large future losses more often than we can accept. To answer that question we need to speficy the likelihood we can accept, say, at 1%. 

This case study uses the `sp500` dataset that covers day-to-day returns for 11 years to illustrate how we can test whether a likelihood is greater or less than a specified value. It illustrates **testing proportions** and how to formulate and carry out a **one-sided hypothesis test**. The case study is a continuation of case study 5A, using the same data.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


# Part II: REGRESSION ANALYSIS

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


# PART III: PREDICTION

## CH13 Predicting used car value with linear regressions  
For how much can we expect to sell our used car? We want to sell our 10-year-old Toyota Camry in the Chicago area. We examine ad prices of similar cars in the area to predict the future selling price. Our `used-cars` dataset includes data from 2018, on the price of a single model with various features (specific type of car, date of manufacture, odometer, condition, etc.). After selecting several predictor variables we build five models. We apply two methods (BIC and k-fold cross-validation) to pick the best model for our point prediction. We find a wide prediction interval and deal with external validity.  

This case study illustrates the main issues we need to address in **predictive data analysis** and the **logic of model selection**, the use of **cross-validation**, **prediction intervals**.


## CH14 Predicting used car value: log prices  
How can we decide whether we should use log prices in a model to predict the future value of our used car? We want to sell our 10-year-old Toyota Camry in the Chicago area. We examine ad prices of similar cars in the area to predict the future selling price. Our `used-cars` dataset includes data from 2018, on the price of a single model with various features (specific type of car, date of manufacture, odometer, condition, etc.). We have five prediction models. After examining the relationship between the price variable and the age of the car, we transform prices to log prices and run our best prediction model. We find that the prediction becomes more uncertain.  

This case study illustrates **whether to take logs of y in regression analysis** and, if yes, what to do with such a prediction.  

## CH14 Predicting AirBnB apartment prices: selecting a regression model
London, UK is a popular tourist destination for business and leisure. We want to predict the rental price of an apartment offered by AirBnB in Hackney, a London borough. We use the `airbnb` dataset that includes rental prices for one night in March 2017 from the area. After sample design, we examine interactions between price and several quantitative and binary predictor variables. We build eight linear regression models and run LASSO on the most complex one. After comparing these models according to various measures of fit, we select the best and run post-prediction diagnostics to we evaluate its predictive performance. We find that our best model could make large errors when predicting the rental price of an apartment.

This case study illustrates the use of a **holdout sample** and the various **methods of building regression models**.  

## CH15 Predicting used car value with regression trees
For how much can we expect to sell our used car? We want to sell our 10-year-old Toyota Camry and examine ad prices of similar cars from the Chicago and Los Angeles areas to predict the future selling price. Our `used-cars` dataset includes data from 2018, on the price of a single model with various features (specific type of car, date of manufacture, odometer, condition, etc.). We examine how the various features of used cars are related to their sales price. We grow seven regression trees by CART and run two linear regressions. Finally, we evaluate the predictive performance of the models by the test set RMSE *and find that the best regression tree is the one that we grew large and pruned*.

This case study illustrates how we can build a **regression tree model** with the help of a **CART algorithm** and how such a model would overfit the original data.  

## CH16 Predicting apartment prices with random forest
London, UK is a popular tourist destination for business and leisure. We want to build the best model to predict the rental price of an apartment offered by AirBnB in London. We use the `airbnb` dataset that includes rental prices for one night in March 2017 from the area of Greater London. We define the best model as the one that has the lowest average squared error. Using apartment location and various features of accommodation as predictors, we carry out feature engineering. After building two random forest models, we construct and compare seven models including two built with gradient boosting machine method (GBM).

This case study illustrates prediction with **random forest** and **boosting** and the evaluation of such predictions.



## CH17	Predicting firm exit: probability and classification

## CH18	Forecasting daily ticket sales for a swimming pool

## CH18	Forecasting a house price index


# PART IV: CAUSAL ANALYSIS


## CH19	Food and health

## CH20	Working from home and employee performance

## CH20	Fine tuning social media advertising

## CH21	Founder/family ownership and quality of management

## CH22	How does a merger between airlines affect prices?

## CH23	Import demand and industrial production

## CH23	Immunization against measles and saving children

## CH24	Estimating the effect of the 2010 Haiti earthquake on GDP

## CH24	Estimating the impact of replacing football team managers
