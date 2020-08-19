---
layout: single
classes: wide
title: "Data and code"
permalink: /data-and-code/
author_profile: false
redirect_from:
  - /md/
  - /data-and-code.html
---


{% include base_path %}

>## *Publish the data and code or it didn't happen* [*](http://freerangestats.info/blog/2020/05/30/implausible-health-data-firm)


Get the raw data and the cleaning codes that created the datasets used for analyis.


**NOTE: codes and data should be made available in the Fall 2020. Please check back in October 2020**


## Getting Data

You have two options to get the datasets for our case studies.

1. Download all the data [Data-all](data-zip-all). Note that this is a very large zipped file - `release 1.0 (2020-11-21)`
2. Download data one by one [from the Datasets page](/datasets)



## Getting code

You have two options to get code for our case studies.

1.  Download all code in [R](code-zip-r), [Stata](code-zip-stata), [Python](code-zip-python) --- `release 1.0 (2020-11-21)`
2.  Download code one by one [from the Case studies page](/casestudies)


## Folder setup
**First**, start by setting up a folder for this textbook, this can sit anywhere. Let us call this da_textbook.

**Second**, there should be two main folders:

One folder for code (and output):   
`da_textbook/da_case_studies`

Another folder for data (clean, raw and cleaning codes).   
`da_textbook/da_data_repo`

**Third**, in the data folder, just copy downloaded dataset folders, such as  
`da_textbook/da_data_repo/hotels-vienna`

It will have two subfolders: `clean` and `raw`, where the `clean` will include the cleaner filers and variable description, `VARIABLES.xls`.

**Fourth**, in the code folder, each case study will have a folder, such as  
`da_textbook/da_case_studies/ch07-hotel-simple-reg`

This folder will host all the codes in **R**, **Stata** and **Python (notebook)**, like
1. ch07-hotel-simple-reg_intro.do
2. ch07-hotel-simple-reg_intro.R
3. ch07-hotel-simple-reg_intro.ipynb

This is where the  `/output` folder will be created (empty when you start) that *will* have all graps and tables produced from code. 

**Fifth** make sure to have the folder `ch00-tech-prep` downloaded and copied into `da_case_studies/`.   
This folder has all the codes to install necessary packages, and settings.   
If you get the whole code package, it is automatically included. 


## Setting up to run code
This textbook is coding language neutral. Our code is written in all three most widely used tools for data analysis. [See our brief summary](/languages/)

[How to set up for Stata?](/howto-stata/)  
[How to set up for R?](/howto-r/)  
[How to set up for Python?](/howto-python/)  
