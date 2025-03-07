## Overview

complete-cases-tool.qmd is a tool used to evaluate the number of complete cases for every possible combination of variables a data set, to help the user decide which variables to keep and which to drop to maximize sample size.

## Motivation

When doing complete case analysis, researchers must drop participants that are missing values in one or more of the variables included in their model. For this reason, some combinations of variables may result in a smaller sample size than others due to varying degrees of missingness across variables. In some cases, a researcher must make a decision about which variables are most important to keep in their study while taking into consideration how inclusions of those variables will affect the number of complete cases, and in turn, the final analytical sample size. This script was designed as a tool to help in that decision. A user can import their data, run this script, and obtain an output that consists of a table that lists every possible combination of variables present in the data set and the corresponding number of complete cases for each given combination.

## Usage

The user needs to provide their data and specify the minimum number of variables they would like to keep in their final data set.

``` r
# create a data frame object containing your data
data <- read.csv(file  = 'path/to/data.csv')

# specify the minimum number of variables that must be kept
min_num_vars <- ... # replace ... with integer
```
Please see example.qmd for an example of how to use this tool, using the Iris data set

