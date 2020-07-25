---
title: "Part I: DATA EXPLORATION"
author_profile: false
collection: casestudies
---
 
## CH01A Finding a good deal among hotels: data collection
Vienna, Austria is a popular tourist destination for business and leisure. From the hundreds of places that offer accommodation, we want to pick a hotel that is underpriced relative to its location and quality for a weekday in November 2017. Can we use data to help this decision? What kind of data would we need, and how could we get it?

This case study illustrates how to collect appropriate data from the web on multiple offers. It describes what we want from such data and what data source we would need. The data is collected by **web scraping**, and it results in a single **data table.** It discusses the **quality of the data** from the perspective of the question and how it is determined by the way the data was born. There is no dataset to analyze in this case study in this chapter. Subsequent case studies (2A, 3A, 7A, 8A, 9B, 10B) will use the data desctibed here to illustrate steps of data analysis that lead to ultimately answering the main question.

 
## CH01B Comparing online and offline prices: data collection
Do online and offline prices of the same products tend to be the same? To answer that question, appropriate data was collected as part of the Billion Prices Project (BPP; http://www.thebillionpricesproject.
com), an umbrella of multiple projects that collect price data for various purposes using various methods.

This case study illustrates how to combine different data collection methods and what are the challenges with such data collection. It discusses how products were selected and how prices were measured, and what those methods imply for coverage of observations and reliability of variables. There is no dataset to analyze in this case study. Case study 6A uses the data described here to investigate whether online and offline prices tend to be the same.

## CH01C Management quality: data collection
How different are firms and other organizations in the terms of management practices? Is the quality of management related to how large the firms are? Is it affected by whether the owners are the founders or their family? To answer these, and many related, questions, appropriate data was collected on the quality of management of many organzations by the World Management Survey (WMS; https://worldmanagementsurvey.org/), an international research intitative to measure the differences in management practices across organizations and countries.

This case study illustrates how to collected data by surveys. It discusses **sampling** and its practical issues, and how to use a set of survey questions to measure and abstract concept such as the quality of management. There is no dataset to analyze in this case study. Case studies 4A and 21A use the data described here to investigate how management quality is related to firm size and how it is affected by ownership.

## CH02A Finding a good deal among hotels: data preparation
Vienna, Austria is a popular tourist destination for business and leisure. From the hundreds of places that offer accommodation, we want to pick a hotel that is underpriced relative to its location and quality for a weekday in November 2017. What kind of variables could we consider during our search for a good deal? We look at qualitative and quantitative variables and create a data table that we can work with.  

This case study illustrates how to find problems with observations and variables and uses the `hotels-vienna` dataset. It shows how to create a **tidy data table** and how to deal with **missing values** and **duplicates**. It allows instructors to demonstrate the importance of **data cleaning** and the common **steps of data wrangling**.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH02B Displaying immunization rates across countries
Immunization against measles is an effective way to prevent the disease and may save the lives of children. But how do various countries fare in terms of their immunization rate? We use the World Development Indicators data website maintained by the World Bank to look at countries’ annual immunization rate and GDP per capita.  

This case study illustrates how to store **multi-dimensional data**. It uses the `world-bank-immunization` dataset and shows a data structure focusing on two ID variables (country and year) and two other variables (immunization rate and GDP per capita). It allows instructors to demonstrate **xt panel data tables in long and wide formats**.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch02C Identifying successful football managers
The English Premier League (EPL) is the top football division in England and we want to identify its most successful football manager. Covering 11 years, the `football` dataset covers  all games played in the EPL and data on managers, including which team they worked at and when. We create a workfile by joining two different data tables. After defining the measure of success as average points per game, we identify the most successful managers.  

This case study introduces how to prepare data for analysis and illustrates linking data tables with different kinds of observations. It shows how to combine two data sources and what kinds of problems can arise while doing so. It allows instructors to demonstrate entity resolution, relational data, tidy data tables, and linking data tables.

**Code**:   [**Stata**](https://github.com/gabors-data-analysis/da_case_studies/blob/master/ch02-football-manager-success/ch02-football-manager-success.do) or [**R**](https://github.com/gabors-data-analysis/da_case_studies/blob/master/ch02-football-manager-success/ch02-football-manager-success.R) or [**Python**](clink) or  [ALL](link)  
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  

![pep-and-fergie](/images/pep-and-fergie.jpg){:height="50%" width="50%"}

 [source](https://www.soccerladuma.co.za/news/articles/international/categories/english-premier-league/sir-alex-ferguson-sends-pep-guardiola-a-warning/228353)


## Ch03A Finding a good deal among hotels: data exploration
Vienna, Austria is a popular tourist destination for business and leisure. We search for a good deal on a weekday in November 2017 among hotels located in the center of Vienna. Using the `hotels-vienna` dataset, we explore the most important variables needed for our analysis with a focus on distribution of hotels in quality and in distance to the city center. We find and manage extreme values of price to create an ultimate sample of hotels.  

![Vienna](/images/vienna1.jpg){:height="70%" width="70%"}


This case study shows the description of distributions and their use in identifying problems in the data. It illustrates the steps of exploratory data analysis and introduces guidelines for data visualization. It illustrates the design of histograms as well as layers of a graphical object.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch03B Comparing hotel prices in Europe: Vienna vs London
How can we compare hotel markets over Europe and learn about characteristics of hotel prices? Using the `hotels-europe` dataset, we pick Vienna and London and focus on 3-4 star hotels located in the city center and compare the distribution of prices for a weekday in November 2017. From our summary statistics and visualized distributions we conclude that hotel prices in London tend to be substantially higher on average and more spread than in Vienna.  

The case study shows some of the most important descriptive statistics for quantitative variables and illustrates the comparison of distributions and the use of histograms and density plots.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch03C Measuring home team advantage in football
Is there such a thing as home team advantage in professional football? Using the `football` dataset, we examine whether and to what extent football teams of the English Premier League (EPL) tended to perform better if they played in their home stadium during the 2016/17 season using the football dataset.  After creating variables and presenting summary statistics we find that soccer teams while playing on their home turf won almost 50% of the time and lost only about 30% of the time.  

The case study shows the use of exploratory data analysis to answer a substantive question and introduces guidelines to present statistics in a good table.

## Ch03D Distributions of body height and income
We look at population data collected by the Health and Retirement Study in the U.S.A. in 2014 (`height-income-distributions` dataset), and show how the height of women aged 55-60 can be described by the normal distribution. For an approximately lognormal distribution, we look at the distribution of household income among households of women aged 55-60 collected by the same study.  

![income](/images//Ch03_figures/ch03-figure-11b-hist-income-log.png){:height="50%" width="50%"}

This case study shows two everyday examples for theoretical distributions, with a focus on normal and lognormal distributions.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## Ch04A Management quality and firm size: describing patterns of association
Are larger companies better managed? We choose one country (Mexico) and use the World Management Survey data -- `wms-management-survey` dataset from 2013 to explore the association between management quality and firm size. By creating a management score to capture the quality of management and using employment to measure firm size, we examine various conditional statistics and informative visualizations. We find that larger manufacturing firms in Mexico are better managed but as the positive correlation is not strong and it varies across industries.

![wms](/images//Ch04_figures/ch04-figure-6b-wms-mex-violin-mgmt-emp3bins.png){:height="50%" width="50%"}

This case study shows what we can do to uncover patterns of association when both y and x are quantitative variables. It illustrates conditional probabilities, various aspects of conditional distributions and shows how to create informative figures by visualizing various kinds of comparisons (scatterplot, bin scatter, box plots).

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH05A What likelihood of loss to expect on a stock portfolio?
Can we find out the future likelihood of a large loss on a stock portfolio based on data from the past? We choose the S&P 500 stock market index as our investment portfolio, and use the `sp500` dataset that covers day-to-day returns for 11 years. After defining large daily loss as an at least 5% drop in returns from one day to another, we search for the proportion of days with large losses. We construct a 95% confidence interval and find that in the general pattern represented by the 11-year history of returns, large daily losses occur with a 0.2 to 0.8 percent chance. However, we find that external validity may not be high and acknowledge that in the future, large daily losses may have a higher probability than 0.8 %.

![bootsrap](/images/bootstrap.jpg){:height="30%" width="30%"}

This case study introduces the concept of repeated samples, standard deviation and confidence intervals. It shows how to make statistical inference in two ways, using the bootstrap method and using a formula for the standard error. It also illustrates how to think about external validity in general.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH06A Comparing online and offline prices: testing the difference
Do online and offline prices of the same products tend to be the same? Using the `billion-prices` dataset, we examine online and offline prices of retail products in the U.S. in 2015-16. We translate our question to an inquiry about a statistic (average difference). First, we form one hypothesis: online versus offline price difference is zero (the null) and not zero (the alternative). After carrying out a hypothesis testing, looking at the p-value as well as at the 95% CI, we find that we can’t reject the null. Second, we test multiple hypotheses. We look at 16 retail stores in the US and for each we test whether the average price differential is zero. After finding that the average online-offline price difference is not zero in some of the retail chains in the data, we argue that the multiple tests may reveal artificial features of the data (measurement error).

This case study introduces the process of hypothesis testing: how to define the statistic of interest, the null, and the alternative. It shows how we can generalize a decision from the population of products represented by the data to the population of products we are interested in. It allows instructors to demonstrate the use of the t-test and the p-value and testing multiple hypotheses.


**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)  


## CH06A Testing the likelihood of loss on a stock portfolio
How can we test whether our stock portfolio is likely to suffer large future losses more often than we can accept? Our portfolio is the S&P 500 stock market index and we use the `sp500` dataset that covers day-to-day returns from 2006 to 2016. First, we define large daily loss as an at least 5% drop in returns from one day to another. Then, we assume that we accept such losses as long as they are less frequent than 1% of the days. We form our alternative hypothesis that the proportion of days with large losses is less than 1% and the null that covers all other possibilities. After calculating the p-value, we reject the null (and conclude that large losses occur less frequently than one percent of the days.)

This case study allows instructors to demonstrate a one-sided hypothesis test.

**Code**: [**Stata**](link) or [**R**](ch07-hotel-simple-reg_intro.R) or [**Python**](clink) or [ALL](link).
**Data**: [hotels-vienna](link-hotels-vienna).
**Graphs**: [.png](ch02A-png-zip) or [.eps](ch02A-eps-zip)
