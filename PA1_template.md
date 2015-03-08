---
title: "Reproducible Research: Peer Assessment 1"
output: 
  html_document:
    keep_md: true
---



## Setup the R environment

The following **(i)** removes (almost) everything in the working `R` environment, **(ii)** loads the contributed `R` package `knitr` and sets its global option `echo` for all `R` code chunks to `TRUE`, and **(iii)** sets the working directory. Unless otherwise specified, `opts_chunk$set(echo=TRUE)` requires `R` through `knitr` to include the `R` source code in the output file. 


```r
# REMOVE ALMOST EVERYTHING IN THE WORKING ENVIRONMENT
rm(list=ls(all=TRUE))
# LOAD THE knitr PACKAGE
library(knitr)
# SET GLOBAL OPTION echo TO TRUE
opts_chunk$set(echo=TRUE)
# SET WORKING DIRECTORY
setwd("C:/Work/Personal/Personal/Coursera/5-ReproducibleResearch/PeerAssessment1")
```



## Loading and preprocessing the data

always unzip the file and override activity.csv- run time OK.


```r
unzip(zipfile="activity.zip")
data <- read.table(file="activity.csv", header=TRUE, sep=",", 
	colClasses=c("numeric","character","integer"))
head(data)
```

```
##   steps       date interval
## 1    NA 2012-10-01        0
## 2    NA 2012-10-01        5
## 3    NA 2012-10-01       10
## 4    NA 2012-10-01       15
## 5    NA 2012-10-01       20
## 6    NA 2012-10-01       25
```

```r
summary(data)
```

```
##      steps            date              interval     
##  Min.   :  0.00   Length:17568       Min.   :   0.0  
##  1st Qu.:  0.00   Class :character   1st Qu.: 588.8  
##  Median :  0.00   Mode  :character   Median :1177.5  
##  Mean   : 37.38                      Mean   :1177.5  
##  3rd Qu.: 12.00                      3rd Qu.:1766.2  
##  Max.   :806.00                      Max.   :2355.0  
##  NA's   :2304
```


## What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
