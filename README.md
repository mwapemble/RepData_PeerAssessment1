# Reproducible Research: Peer Assessment 1
Matthew Pemble  
20 December 2015 

## Introduction

This is the README.md file for the 20 Dec 2015 submission by Matthew Pemble of the first peer assessment for the Johns Hopkins "Reproducible Research" Coursera Course.

## Data
The data set provided consists of the number of steps taken by a data subject over 5 minute intervals, between 1 Oct 2012 (although that day has no valid data) and 30 Nov 2012.  

The data set was provided as part of the assignment material and no attribution was provided.

## Preprocessing
No data pre-processing was conducted.

## Analysis
The analysis consisted of a number of defined tasks:

- Calculate the total number of steps taken per day.
    + Display a histogram of the results.
    + Report the mean of the total number of steps.
    + Report the median of the total number of steps.
- Derive the average daily activity pattern.
    + Display a line plot of the average number of steps taken per interval.
    + Report which interval, on average, contained the maximum number of steps.
- Replace the missing values in the original data with sensible alternatives.
    + Select a strategy for replacing the data - median data per interval was selected.
    + Modify the dataset.
    + Repeat the initial histogram, mean & median calculations.
    + Report on any differences.
        + Note that some additional calculations and displays were provided to show that the median data was valid.
- Report on any differences between activities at the weekend and during the week, using the modified dataset.
    + Make a panel plot of line graphs showing the average number of steps taken per interval at the weekend and during the week.
    
## Acknowledgements

As usual, function and syntax tips were gained from a variety of sources, including the lecture notes and examples from the previous course material:  

1. Books  
    + Kabacoff, Robert; R in Action  
    + Knell, Robert; Introductory R 
    
1. Websites  
    + R4stats.com  
    + blog.echen.me (particularly for ggplot2 - not used in the end)  
    + stackoverflow.com  
    + r-bloggers.com  
    + rstudio.com (package instructions & markdown cheat sheet)  
    + dummies.com (reminded me about the layout option for xyplot() )