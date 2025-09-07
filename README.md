# birthweight-analysis

# Low & Very Low Birthweight Analysis (2014-2018)

**Goal** Explore low-birthweight rates by race/ethnicity and highlight disparities.

# Libraries

library(tidyverse)
library(arsenal)
library(gtsummary)
setwd("/Users/fangwang/Downloads/P8130 Biostatistical Methods I/birthweight-analysis")


# Dataset

data = read.csv("./low-birthweight-by-race-ethnicity-2014-2018.csv")|>
  janitor::clean_names()


# publication-ready table using tbl_summary()

table = tbl_summary(data)
table
