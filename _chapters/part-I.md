---
title: "Part I: DATA EXPLORATION"
author_profile: false
collections: chapters
toc: true
toc_label: "PART I: DATA EXPLORATION"
toc_sticky: true
---

## Chapter 01: Origins of Data  
This chapter is about the definition of data, data collection, and data quality.
The chapter starts by introducing **key concepts of data**. It then describes the most important **methods of data collection** used in business, economics, and policy analysis, such as **web scraping**, **using administrative sources**, and **conducting surveys**. We introduce aspects of data quality, such as **validity and reliability of variables** and **coverage of observations**. We discuss how to assess and link data quality to how the data was collected. We devote a section to **Big Data** to understand what it is and how it may differ from more traditional data. This chapter also covers **sampling**, incuding **random sampling** and biases due to **noncoverage** and **nonresponse**, as well as **ethical issues** and some **good practices in data collection**.  

## Chapter 02: Preparing Data for Analysis  
This chapter is about preparing data for analysis: how to start working with data. 
First, we clarify some concepts: **types of variables**, **types of observations**, **data tables**, and **datasets**. We then turn to the concept of **tidy data**: data tables with the same kinds of observations. We discuss potential issues with observations and variables, and how to deal with those issues. We describe **good practices for the process of data cleaning** and discuss the additional **challenges of working with Big Data**.  

## Chapter 03: Exploratory Data Analysis  
The chapter starts with **exploratory data analysis** is important. It then discusses some basic concepts such as **frequencies**, **probabilities**, **distributions**, and **extreme values**. It includes guidelines for producing informative graphs and tables for presentation and describes the most important **summary statistics**. The chapter and its appendix also cover some of the most important **theoretical distributions** and their uses.  

## Chapter 04: Comparison and Correlation
Most methods of data analysis are based on comparing values of one variable, *y*, across observations with different values of another variable, *x*, or more such variables. This chapter instroduces simple methods of such comparison.
We start by emphasizing that we need to define both *y* and *x* precisely for meaningful comparisons, and we need to measure them well. We introduce **conditioning**, and we discuss **conditional comparisons**, or further conditioning, which takes values of other variables into account as well. We discuss **conditional probabilities**, **conditional distributions**, and **conditional means**. We introduce the related concepts of **dependence**, **mean-dependence**, and we introduce **covariance** and **correlation**. Throughout the chapter, we discuss informative **visualization** of the various kinds of comparisons.

## Chapter 05: Generalizing from Data  
This chapter introduces the conceptual issues with generalizing results from our data to the general pattern we care about and methods of statistical inference.
We start by discussing the **two steps of the process of generalization**: generalizing from the data to the **general pattern our data represents**, such as a population, and assessing how the **general pattern that is relevant for the situation we care about** relates to the general pattern our data represents. The first task is **statistical inference**, the second is assessing **external validity**. We introduce the conceptual framework of **repeated samples** and **estimation**. We introduce **the standard error** and **the confidence interval** that quantify the uncertainty of this step of generalization. We introduce two methods to estimate the standard error, **the bootstrap** and **the standard error formula**. Discussing external validity, we acknowledge that there are no readily available methods to quantify the uncertainty of this step of generalization, but we discuss how we can think about it and how we may use the results of additional data analysis to assess it.

## Chapter 06: Testing Hypotheses  
This chapter introduces the logic and practice of testing hypotheses. 
We describe the **steps of hypothesis testing** and discuss two alternative ways to carry it out: one with the help of a **test statistic** and a **critical value**, and another one with the help of a **p-value**. We discuss how decision rules are derived from our desire to control the likelihood of making erroneous decisions (**false positives** and **false negatives**), and how **significance levels**, **power**, and **p-values** are related to the likelihood of those errors.  We focus on testing hypotheses about averages, but, as we show in one of our case studies, this focus is less restrictive than it may appear. The chapter covers **one-sided versus two-sided alternatives**, issues with **testing multiple hypotheses**, the perils of **p-hacking**, and some issues with testing on Big Data.  

