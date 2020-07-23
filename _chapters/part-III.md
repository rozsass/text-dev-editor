---
title: "Part III: PREDICTION"
author_profile: false
collections: chapters
toc: true
toc_label: "PART III: PREDICTION"
toc_sticky: true
---

## Chapter 13: A Framework for Prediction  
This chapter introduces a framework for prediction. We discuss the distinction between various types of prediction, such as **quantitative predictions**, **probability predictions**, and **classification**, and we focus on the first of these. We introduce **point prediction versus interval prediction**; we discuss the **components of prediction error** and how to find the best prediction model that will likely produce the best fit (smallest prediction error) in the live data, using observations in the original data.  
We introduce **loss functions** in general, and **mean squared error (MSE)** and its **square root (RMSE)** in particular, to evaluate predictions. We discuss three ways of finding the best predictor model: using all data and **the Bayesian Information Criterion (BIC)** as the measure of fit, using **training–test splitting** of the data, and using **k-fold cross-validation**, which is an improvement on the training–test split. We discuss how to assess and, if possible, improve the external validity of predictions. We close the chapter by discussing what **machine learning** means.  

## Chapter 14: Model Building for Prediction  
This chapter discusses how to **build regression models for prediction** and how to evaluate the predictions they produce. With respect to model building, we discuss whether and when it’s a good idea to **take logs of the y variable** and what to do with such a prediction, how to select variables out of a large pool of candidate x variables, and how to decide on their functional forms. We introduce **LASSO**, an algorithm that can help with variable selection.  
With respect to **evaluating predictions**, we discuss why we need a **holdout sample** for evaluation that is separate from all of the rest of the data we use for model building and selection.  
We close this chapter with a discussion on the additional opportunities and challenges **Big Data** brings for **predictive analytics**.  

## Chapter 15: Regression Trees  
This chapter introduces **the regression tree**, an alternative to linear regression for prediction purposes that can find the most important predictor variables and their interactions and can approximate any functional form automatically. Regression trees split the data into small bins (subsamples) by the value of the x variables. For a quantitative y, they use the average y value in those small sets to predict ˆy.  
We introduce the regression tree model and the most widely
used **algorithm to build a regression tree model**. Somewhat confusingly, both the model and the algorithm are called **CART** (for classification and regression trees), but we reserve this name for the algorithm. We show that a regression tree is an intuitively appealing method to model nonlinearities and interactions among the x variables, but it is rarely used for prediction in itself because it is prone to overfit the original data. Instead, the regression tree forms the basic element of very powerful prediction methods that we’ll cover in the next chapter.  

## Chapter 16: Random Forest and Boosting  
This chapter introduces two ensemble methods based on regression trees: the random forest and boosting. We start by introducing the main idea of ensemble methods: combining results from many imperfect models can lead to a much better prediction than a single model that we try to build to perfection. Of the two methods, we discuss **the random forest (RF)** in more detail. The random forest is perhaps the most frequently used method to predict a quantitative y
variable, both because of its excellent predictive performance and because it is relatively simple to use. Even more than with a single tree, it is hard to understand the underlying patterns of association between y and x that drive the predictions of ensemble methods. We discuss some diagnostic tools that can help with that: **variable importance plots**, **partial dependence plots**, and examining the **quality of predictions in subgroups**.  
Finally, we briefly introduce the idea of **boosting**, an alternative approach to make predictions based on an ensemble of regression trees. There are various boosting methods, and they can produce even better predictions. However, it
is hard to choose from the various methods, and none of them are easy to understand or to use. We illustrate the power of boosting through the performance of the **gradient boosting machine (GBM) method**.  

## Chapter 17: Probability Prediction and Classification  
This chapter introduces the framework and methods of probability prediction and classification analysis for binary y variables. **Probability prediction** means predicting the probability that y = 1, with the help of the predictor variables. **Classification** means predicting the binary y variable itself, with the help of the predictor variables: putting each observation in one of the y categories, also called classes. We build on what we know about probability models and the basics of probability prediction from Chapter 11. In this chapter, we put that into the framework of predictive analytics to arrive at the best probability model for prediction purposes and to evaluate its performance. We then discuss how we can turn probability predictions into classification with the help of a **classification threshold** and how we should use a **loss function** to find the **optimal threshold**.  
We discuss how to evaluate a classification making use of a **confusion table** and **expected loss**. We introduce **the ROC curve**, which illustrates the trade-off of selecting different classification threshold values. We discuss how we can use random forest based on classification trees. Finally, we note the potential issues with the probability prediction and classification of rare events.  

## Chapter 18: Forecasting from Time Series Data  
This chapter discusses forecasting: prediction from time series data for one or more time periods in the future. The focus of this chapter is forecasting future values of one variable, by making use of past values of the same variable, and possibly other variables, too. We build on what we learned about time series regressions in Chapter 12. We start with **forecasts with a long horizon**, which means many time periods into the future. Such forecasts use information on trends, seasonality, and other long-term features of the time series. We then turn to **short-horizon forecasts** that forecast y for a few time periods ahead. These forecasts make use of **serial correlation** of the time series of y besides those long-term features. We introduce **autoregression (AR)** and **ARIMA models**, which capture the patterns of serial correlation and can use it for short-horizon forecasting.  We then turn to using other variables in forecasting, and introduce **vector autoregression (VAR) models** that help in forecasting future values of those x variables that we can use to forecast y. We discuss how to carry out **cross-validation in forecasting** and the specific challenges and opportunities the time series nature of our data provide for assessing external validity.  