---
title: "Part III: PREDICTION"
author_profile: false
collection: casestudies
---


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
