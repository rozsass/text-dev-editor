---
permalink: /howto-stata/
title: "How to set up your computer for Stata"
excerpt: "Set up system, get Stata, create a project"
author_profile: false
redirect_from:
  - "/nmp/"
  - "/nmp.html"
---

## Code language versions
1. **Stata** -- We used v15.1, but all code should work for versions above 13.0. We saved data in the Stata 13 version.

## Organization
1. Each case study has a separate folder.
2. Within case study folders, codes in different languages are simply stored together.
3. Some intermediary files (csv, dta, rds) may be saved there, too.
4. Currently output is not stored here

## Get Stata
1. You will need a Stata license to use it. Your institution may have access, check for that.
2. You may ask for a [student license](https://www.stata.com/customer-service/short-term-license/), too.


## How to run case studies in Stata

1. Create a folder for this textbook (such as `my-data-analysis`)
2. Within this folder, create a folder `my-data-analysis/data-repo` this should include all data folders.
3. Create another folder  `my-data-analysis/case-studies` this will host all case studies
4. When you start up stata, set the working directory as your main folder (`cd my-data-analysis`)
5. When you run a code, just use add the folder name `do case-studies/ch02-football-manager-success/ch02-football-manager-success.do`
