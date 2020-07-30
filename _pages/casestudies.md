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
Will our investment portfolio suffer a large loss with a higher chance than what we can accept? When we want to know what's the likelihood of large future losses on our portfolio, we can use the confidence interval to quantify the uncertainty from estimating it from data on past returns. But we can ask a more pointed question, too: whether our stock portfolio is will suffer large future losses more often than we can accept. To answer that question we need a different procedure: testing a hypothesis. 

This case study uses the `sp500` dataset that covers day-to-day returns for 11 years to illustrate how we can test whether a likelihood is greater or less than a specified value. It illustrates **testing proportions** and how to formulate and carry out a **one-sided hypothesis test**. The case study is a continuation of case study 5A, using the same data.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


# Part II: REGRESSION ANALYSIS

## CH07A Finding a good deal among hotels with simple regression
How can we find the hotels that are underpriced relative to their distance from the city center? Continuing the previous case studies that resulted in a clean data table ready for analysis, we need to uncover how hotel price is related to distance to the city center to know what price to expect at what distances. Then can we identify hotels that are the most underpriced compared to their expected price.

This case study uses the `hotels-vienna` dataset to illustrate regression analysis with one right-hand-side variable. It shows the use of **bin scatters** and **lowess non-parametric regressions** that reveal qualitative patterns of association. In order to find out the quantitative relationship between distance and average price, we apply **simple linear regression**. The case study illustrates the use of **predicted values** and **regression residuals** 


## CH08A Finding a good deal among hotels with non-linear function
Continuing our search for the best hotel deals in Vienna, we would like to uncover the shape of the price-distance association to get at the best estimates of expected prices at various distances. But what's the best way to compare prices? Should we compare their absoulte values, or should we aim for a relative comparison, such as percent differences? And how can we do the latter in a regression using cross-sectional data?

This case study again uses the `hotels-vienna` dataset, to illustrate linear regression analysis with the use of **logarithms**. It shows whether and why it may make sense to take logs of the variables in the regression, and how to estimate, and interpret the results of, and choose from **level-log** regressions, **log-level** regressions, and **log-log** regressions. 


## CH08B How is life expectancy related to the average income of a country?
People tend to live longer in richer countries. How long people live is usually measured by life expecatncy; how rich a country is usually captured by its yearly income, measured by total GDP or GDP per capita. But what's the shape of the patterns of association? Is the same percent difference in income related to the same difference in how long people live among richer countries and poorer countries? Finding the shape of the association helps benchmarking life expectancy among countries with similar levels of income and identify countries where people tend to live especially long or especially short lives for their income.

This case study uses data from the `worldbank-lifeexpectancy` dataset based on the World Development Iindex database available at the World Bank webside. It examines cross-sectional data from a single year, 2017, for 182 countries. The case study illustrates the choice between **total and per capita measures** (here GDP), regressions with **variables in logs**, and two ways to model nonlinear patterns in the framework of the linear regression: **piecewise linear splines**, and **polynomials**. It also illustrates whether and how to use **weights** in regression analysis, and what that choice implies for the correct interpretation of the results. The case study also shows how to use **informative visualization** to present the results of regressions.


## CH08C Measurement error in hotel ratings
When we search for a good deal among hotels, we care about hotel quality as well as distance to the city center. But hotel quality is difficult to measure. Online price comparison websites include customer ratings, and the average of those ratings can serve as good measures. But some averages are based on very few ratings while others are based on hundreds or thousands of ratings. Should we be concerned about ratings coming from very few customers? In particular, what are the consequences of that feature of the data on the results of regression analysis?

This case study again uses the `hotels-vienna` dataset, to illustrate the consequences of measurement error for regression analysis. In particular, it shows the effect of **classical measurement error** in the right-hand-side variable on the estimated slope of a simple linear regression. 


## CH09A Estimating gender and age differences in earnings
Do women working in the same occupation tend to earn the same as men? And what's the differences in earnings by age? Understanding these differences may help students know what to expect when choosing a particular career. 

This case study uses the `cps-morg` dataset, a cross-section based on the Current Population Survey (CPS) of the U.S. in 2014. It focuses on a single occupation potentially relevant for many students, "Market research analysts and marketing specialists". The case study illustrates how to estimate the **standard error** of regression coefficients and how to construct and interpret **confidence intervals**. It also shows how to **test hypotheses about regression coefficients**. It also includes the standard way of **presenting regression results** in tables.


## CH09B How stable is the hotel price–distance to center relationship?
We have uncovered the average price - distance association among hotels in a particular city on a particular date. How generalizable is this pattern to other dates, to other cities, and to other types of accommodations?

This case study uses the `hotels-europe` data from Vienna, Amsterdam and Barcelona. It illustrates the various kinds of **issues with external validity**, first focusing on time (different dates), then space (different cities), and groups of observations (different kinds of accommodations).


## CH10A Understanding the gender difference in earnings
Women earn less, on average, than man with similar qualifications. How large is that difference among employees with a graduate degree? How does that difference vary with age? And how much do characteristics of the employer and family circumstances explain of the difference? Understanding the magnitude, patterns, and causes of gender differences in earnings is important from the viewpoint of social equity as well as efficient allocation of labor.  

This case study uses the `cps-morg` dataset to illustrate the use of multiple regression analysis to help understand the sources of differences between groups of observations. The data is a cross-section based on the Current Population Survey (CPS) of the U.S. in 2014, and the sample is restricted to employees with a graduate degree. The case study illustrates how to estimate and intepret the results of a **multiple regression**. It shows how to include **qualitative right-hand-side variables** and **interactions** in the regression, how to interpret their results, and how to use **visualization** to present estimtes of nonlinear patterns. The case study illustrates the difficulty of uncovering causal relationships from the results of multiple regression analysis using cross-sectional data. 


## CH10B Finding a good deal among hotels with multiple regression
We return to estimating a good deal among hotels for the last time in this case study. We want to find the hotels that are underpriced for their quality and distance to the city center. To do so we first need to uncover expected prices at various levels of distance and quality in a way that reflects all important patterns in the data. Then can we look for hotels that are the most underpriced relative to their expected price.

This case study uses `hotels-vienna` dataset to illustrate the use of multiple regression analyis for prediction within a sample and **residual analysis**. It uses the susample of 3-4 star hotels for a single night in Vienna in November 2017. It illustrates the use of nonlinear specification within a multiple regression and how to identify observations with the largest negative residuals. It also illustrates the use of the **y-hat - y plot** to visualize the prediction within the sample and the residuals from the predicted values. 


## CH11A Does smoking pose a health risk?
Are smokers less likely to remain healthy than non-smokers? How about former smokers who quit? 

This case study uses the `share-health` data from the SHARE survey (Survey for Health, Aging and Retirement in Europe). We focus on people who were 50 to 60 years old and said to be in good health in 2011. We look at how they rated their health in 2015 and see who changed their answer to not healthy. This case study illustrates probability models. It shows how to estimate and interpret the results of a **linear probability model** and the uses of **logit** and **probit** models. It compares the linear probability estimates to the estimated **marginal differences** from logit and probit. Finally, it illustrates when and how the different models may result in different **predicted probabilities** and how to compare their fit using **Brier-score** and other measures of fit.


## CH11B Are Australian weather forecasts well-calibrated?
Should we take an umbrella when weather forecast predicts rain? In other words, how should we trust the weather forecast when it predicts a certain the likelihood of rain? For example, is it true that it rains on 20 percent of the days when it says the likelihood is 20 percent?

This short case study uses the `australia-weather-forecast` data covering 350 days in 2015/16 and looks at rain forecast and actual rain for the Northern Australian city of Darwin. The case study illustrates how to construct and interpret a **calibration curve**.


## CH12A Returns on a company stock and market returns
How do monthly returns on a company stock move together with monthly market returns? The strength of this association is a good measure of how risky the company stock is. 

This case study uses the `stocks-sp500` dataset covering 21 years of daily data of many company stocks, focusing on the Microsoft stock and the S&P 500 stock market index (S&P 500). We construct monthly time series of percent returns as the percent change in closing price on the last day of each month. The case study illustrates the use of a simple **time series regression** in changes, focusing on the interpretation and visualization of the results.


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
