---
title: "Reproducible Research: Peer Assessment 1"
output: 
  html_document:
    keep_md: true
---



## Setup the R environment

The following sets the global option `echo` for all `R` code chunks to `TRUE`. Implicitly and unless otherwise specified, this requires `R` through `knitr` to include the `R` source code in the output file. 


```r
# REMOVE ALMOST EVERYTHING FROM THE ENVIRONMENT
rm(list=ls(all=TRUE))
# LOAD THE knitr PACKAGE
library(knitr)
# SET GLOBAL OPTION echo TO TRUE
opts_chunk$set(echo=TRUE)
# SET WORKING DIRECTORY
setwd("C:/Work/Personal/Personal/Coursera/5-ReproducibleResearch/PeerAssessment1")
```



## Loading and preprocessing the data



## What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
