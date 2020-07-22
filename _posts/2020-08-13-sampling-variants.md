---
title: 'Variants of random sampling'
date: 2020-07-13
permalink: /posts/2020/07/sampling-variants/
tags:
  - random sampling
  - ch01
  - in-depth
  - methods

---




There are many variations on random sampling that aim to further improve representation or reduce the costs of data collection. 

## 3 Variants of random sampling

**Stratified sampling** improves on the representative nature of a sample. It starts by specifying large groups in the population, and it applies random sampling within each group. 

**Cluster sampling** starts by specifying small groups, takes a random sample from each of those groups, and collects data from all observations within each selected group. It can greatly reduce data collection cost, for example for in-person interviews that require a lot of traveling. In exchange, cluster samples increase the uncertainty in the data because the number of clusters is a lot smaller than the number of people, thus the sample size is smaller from the point of view of representation. 

**Multi-stage sampling** mitigates this problem by selecting a somewhat larger number of clusters in a first stage and taking a random sample of observations within each cluster instead of including all observations. Some data collection requirements present specific circumstances that may call for further variations on random sampling. 

One example for stratified sampling comes from the `Comparing online and offline prices` case study. People collecting data received instructions to sample a specified number of products (between 10 and 50) in each store, in a stratified manner (by department). To what extent the resulting samples ended up representing the population is an open question here. However, if the purpose of the analysis of comparing online and offline prices, it is this difference that has to be similar in the sample and in  the population of all products. As long as these distributions are similar, other differences are not that important.
