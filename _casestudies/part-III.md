---
title: "Part III: PREDICTION"
author_profile: false
collection: casestudies
---


## CH13 Predicting used car value with linear regressions  
For how much can we expect to sell our used car? In particular, what price should we adverties if we wanted to sell our 10-year-old Toyota Camry in the Chicago area? And what could price we expect if we waited some time? With appropriate data on similar used cars we can estimate various regression models to predict expected price as a function of various features. But how should we select the best regression model for prediction?

This case study uses the `used-cars` dataset that includes data from classified ads of used cars from various cities of the U.S.A. in 2018. We select a single model and a single city. The variables include the ask price and various features (specific type of car, date of manufacture, odometer, condition, etc.). We specify several linear regression models to predict the expected price as a function of car features. This case study illustrates the basic logic of carrying out **predictive data analysis** and **model selection**, emphasizing the need to achieve a good fit in the **live data** by selecting a model using the **original data** and avoiding both **underfitting** and **overfitting** the data. It illustrates the use of a **loss function** such as the **mean-squared error (MSE)** as a measure of fit, and it discusses alternative model selection strategies such as the **BIC**, the **training-test split**, and its improved version, **k-fold cross-validation**. 


## CH14 Predicting used car value: log prices  
Continuing with our example of predicting used car prices, how should we decide on whether to transform our target variable? In particular, we can speficy regression models with log price as well as price as the target variable. How to make predictions about price when the target variable is in logs, and how to choose between models with log price versus price as the target variable? 

This case study uses the `used-cars` dataset with Toyota Camry cars from Chicago in 2018 to illustrate prediction with a log target variable. This short case study illustrates how to use **log cortrection** to predict a *y* variable when the model is specified in *ln(y)* and how to construct appropriate **prediction intervals**. The case study is a continuation of case study 13A, using the same data.


## CH14 Predicting AirBnB apartment prices: selecting a regression model
London, UK is a popular tourist destination for business and leisure. We want to predict the rental price of an apartment offered by AirBnB in Hackney, a London borough. The results of this prediction can help tourists choose an offer that is underpriced for its features or apartment owners to deciding on what price they could expect if they rented out their apartment on AirBnB.  

This case study uses the `airbnb` dataset that includes rental prices for one night in March 2017 from the area. After sample design, we specify linear regressions of varing complexity and a model with LASSO. This case study illustrates the various **methods of building regression models**, including **LASSO**, and the use of a **holdout sample** for **evaluating** the predictive properties of the best model.


## CH15 Predicting used car value with regression trees
Further continuing with our example of predicting used car prices, is there a better method for prediction than regression that can capture nonlinear patterns and interactions between feature variables? In particular, how does prediction from a regression tree compare to prediction from a linear regression?

This case study uses the `used-cars` dataset from 2018 and its combined Chcicago and Los Angeles subsamples on a specific make and type of car, to illustrate regression trees. We grow several regression trees and compare their predictive performance of linear regressions. This case study illustrates how we can build a **regression tree model** with the help of the **CART algorithm**, and how such a model could **overfit** the original data. The case study is a continuation of case studies 13A and 14a, using the same data source but a larger subsample of the observations.


## CH16 Predicting apartment prices with random forest
London, UK is a popular tourist destination for business and leisure. We want to build the best model to predict the rental price of an apartment offered by AirBnB in London. 

We use the `airbnb` dataset that includes rental prices for one night in March 2017 from the area of Greater London. Using apartment location and various features of accommodation as predictors, we carry out feature engineering and build random forest models and gradient boosting machine method (GBM) models. This case study illustrates prediction with **random forest** and **boosting** and the evaluation of such predictions. It shows how to carry out necessary **feature engineering**, how to set various **tuning parameters** for the different models and how those affect the predictions. It also illustrates the use of **variance importance plots** and **partial dependence plots** to help understand the patterns of association that drive the predicitons in these **black box models**. The case study is a continuation of case study 14b, using the same data source but the entire London sample instead of a single borough.


## CH17	Predicting firm exit: probability and classification
Many companies have relationships with other companies, as suppliers or clients. Whether those other companies stay in business in the future is an important question for them. How can we use data on many companies across the years to predict the probability of their exit? And can we classify them into two groups, companies that are likely to exit and companies that are likely to stay in business? 

This case study uses the `bisnode-firms` dataset, a panel dataset with a large number of companies from specific industries in a European country, to illustrate probability prediction and classification. After a good deal of feature engineering we estimate several logit models to predict the probablity of firm exit and compare their performance by 5-fold cross-validation, choose the best model to describe how well it predicts the probabilities on a holdout sample, and use the predicted probabilities and two alternative methods for classification. This case study illustrates how to carry out **probability predictions**, how to evaluate their goodness of fit and other aspects of predictive performance, how to find an **optimal classification threshold** with the help of a loss function usign a formula or model-dependent cross-validation, and how to use **expected loss** and the **confusion table** to evaluate classifications. It illustrates how the **ROC curve** visualizes the trade-offs of false positive and negative decisions at various classification thresholds, and how to use **random forest for probaility prediction and classification**. The case study is also a good example of potential issues with **external validity** of predictions and how we may detect the possibility of such issues in the original data.


## CH18	Forecasting daily ticket sales for a swimming pool
How can we use transaction data to predict the daily volume of sales? In particular, how can we use data on sales terminal data on tickets sold to a swimming pool to predict the number of daily tickets sold for next year? 

This case study uses the `swim-transactions` dataset with transaction-level data from all swimimng pools for many years in Albuquerque, New Mexico, USA, and selects a single swimming pool. The case study illustrates the use of seasonality at various levels in long-term predictions. We aggregate the data to daily frequency, discuss data issues and how to solve them, carry out exploartory data analysis to identify potential interactions between monthly and daily seasonality and the importance of predictable events such as shcool holidays, specify several regression models, and select the best by cross-validation. The case study illustrates the use of **transactions data** in predictive analytics, the specific kinds of **cross-validation with time series data**, the use of **trend** and, especially, **seasonality** in making long-term predictions, the use of the autmated **Prophet** algorithm to find the best model, and how to evaluate the prediction of the best model to understand uncertainty of the prediction and detect problems that further data work and analysis may solve.


## CH18	Forecasting a house price index
How can we use data on past home prices, and possibly other variables, to predict how house prices will move in a particular city in the next months? 

This case study uses the `case-shiller-la` dataset with monthly observations on the Case-Shiller home price index for the city of Los Angeles, California, USA between 2000 and 2017. The dataset also contains monthly time series of the unemployment rate and employment rate. After exploratory data analysis we estimate various ARIMA time series models that use the price index, as well as VAR models that use the unemployment and employment rates as well, and we use appropriate cross-validation to select the best model. The case study illustrates how to make use of **serial correlation** to make short-term forecasts with the help of **ARIMA models**, how to use other variables and their forecasted values in a **vector autoregression (VAR)** model, and how to select the best model by **cross-validation with time series data** that preserves the serial correlation in the data. 
