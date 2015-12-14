# Reproducible Research: Peer Assessment 1
Matthew Pemble  
14 December 2015  

## Loading and preprocessing the data


```r
## Initialise variables
data.directory <- "data"
datafile <- "activity.zip"

## Check to see if there is a data directory
## If not, create it.
if (!file.exists(data.directory)) {
  dir.create(data.directory)
}

## Extract files from zip archive
datafile <- paste(".", data.directory, datafile, sep="/")
if (!file.exists(datafile))
{
  unzip("activity.zip", exdir = data.directory)
}

## Then extract & subset to get the relevant data
activity <- read.csv("data/activity.csv")
```





## What is mean total number of steps taken per day?


```r
require(dplyr)
```

```
## Loading required package: dplyr
## 
## Attaching package: 'dplyr'
## 
## The following objects are masked from 'package:stats':
## 
##     filter, lag
## 
## The following objects are masked from 'package:base':
## 
##     intersect, setdiff, setequal, union
```

```r
day_activity <- group_by(activity, date)
total_day <- summarize(day_activity,tot=sum(steps))
hist(total_day$tot,breaks=10)
```

![](PA1_template_files/figure-html/unnamed-chunk-2-1.png) 

```r
mean(total_day$tot,na.rm=TRUE)
```

```
## [1] 10766.19
```

```r
median(total_day$tot,na.rm=TRUE)
```

```
## [1] 10765
```

## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
