---
title: "Part II: REGRESSION ANALYSIS"
author_profile: false
collections: chapters
toc: true
toc_label: "PART II: REGRESSION ANALYSIS"
toc_sticky: true
---

## Chapter 07: Simple Regression  
In this chapter, we introduce **simple non-parametric regression** and **simple linear regression**.
We discuss nonparametric regressions such as **bin scatters**, **step functions** and **lowess** regressions and their visualization. The larger part of the chapter discusses simple linear regression in detail. We introduce the **regression equation**, how its coefficients are **estimated** in actual data by the method of **ordinary least squares (OLS)**, and we emphasize how to **interpret the coefficients**. We introduce the concepts of **predicted value**, **residual**, and **goodness of fit**, and we discuss the relationship between regression and correlation. We end with a note on the relationship between causation and regression.

## Chapter 08: Complicated Patterns and Messy Data  
The first part of this chapter covers how linear regression analysis can accommodate nonlinear patterns. We discuss transforming either or both the dependent variable and the explanatory variable, such as **taking log**; **piecewise linear spline**; and **quadratic** and **higher-order polynomials**. We discuss whether and when to apply each technique, we emphasize the **correct interpretation of the coefficients** of these regressions and how we may **visualize** their results.  
The second half of the chapter discusses potential issues with regression analysis with **influential observations** and **measurement error in variables**. The chapter closes by discussing whether and how to use **weights in regression analysis**.  

## Chapter 09: Generalizing Results of a Regression
This chapter discusses the methods of generalizing results of a linear regression from our data to the general pattern we care about.
We start by describing the two steps of generalization in the context of regression analysis: **statistical inference** and **external validity**. Then we turn to statistical inference: quantifying uncertainty brought about by generalizing to the general pattern represented by our data. We discuss how to **estimate the standard errors and confidence intervals** of the estimates of the regression coefficients, how to **estimate prediction intervals**, and how to **test hypotheses about regression coefficients**. We introduce **ways to visualize** the confidence interval and the prediction interval together with the regression line, and we introduce the standard way to **present the results of regression analysis** in tables.

## Chapter 10: Multiple Linear Regression  
This chapter introduces **multiple regression**.
We start by discussing why and when we should estimate a multiple regression and how to interpret its coefficients. We then turn to how to construct and interpret **confidence intervals of regression coefficients** and **test hypotheses about regression coefficients**. We discuss the relationship between multiple regression and simple regression and derive the **omitted variable bias**. We explain that piecewise linear splines and polynomial regressions are technically multiple linear regressions without the same interpretation of the coefficients. We discuss how to include **categorical explanatory variables** as well as **interactions** that help uncover different slopes for groups. We include an informal discussion on how to decide what explanatory variables to include and in what functional form. Finally, we discuss why a typical multiple regression with cross-sectional observational data is not a **ceteris paribus** comparison, and that, as a result, it may get us closer to causal interpretation without fully uncovering it.

## Chapter 11: Modeling Probabilities  
This chapter introduces probability models that have a **binary dependent variable**.
It starts with the **linear probability model**, and we discuss the interpretation of its coefficients. Linear probability models are usually fine to uncover average associations, but they may be less good for prediction. The chapter introduces the two commonly used alternative models, **the logit** and **the probit**. Their coefficients are hard to interpret; we introduce **marginal differences** that are transformations of the coefficients and have interpretations similar to the coefficients of linear regressions. We argue that linear probability, logit, and probit models often produce very similar results in terms of the associations with explanatory variables, but they may lead to different predictions. We discuss and compare various measeures of fit for probability models, such as the **Brier-score**, and we introduce the concept of **calibration**. We end by explaining how data analysts can analyze more complicated *y* variables, such as **ordinal qualitative variables** or **duration variables**, by turning them into binary ones and estimating probability models.  

## Chapter 12: Regression with Time Series Data  
In this chapter we discuss the opportunities and challenges brought about by regression analyiss of time series data and how to address those challenges.
The chapter starts by discussing features of time series variables, such as **trends**, **seasonality**, **random walk**, and **serial correlation**. We explain why those features make regression analysis challenging and what we can do about them. In particular, we discuss when it’s a good idea to transform the *y* and *x* variables into differences, or relative differences. We introduce two methods to get appropriate standard error estimates in time series regressions: **the Newey–West standard error estimator** and including the **lagged *y* variable** on the right-hand side. We also discuss how we can estimate delayed associations by adding **lags of *x*** to a time series regression, and how we can directly estimate **cumulative, or long run, associations** in such a regression. 
