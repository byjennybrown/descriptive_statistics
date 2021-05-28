Descriptive\_Statistics
================
by: Jenny Brown
5/28/2021

## Descriptive Statistics

This is an R Markdown document for performing descriptive statistics in
R:

## Load Data

The code below reads a csv file and file.choose open a window to choose
the csv file. Remove the \# from the code below and choose the .csv file
of interest.

``` r
# enter.dataset.name<-read.csv(file.choose())
```

## Descriptive Statistics

Example for cars data set. Changes cars to “enter.dataset.name” chick
Edit\>Find to replace all the cars with “enter.dataset.name”

``` r
#Mean
mean(cars$speed)
```

    ## [1] 15.4

``` r
#Median
median(cars$speed)
```

    ## [1] 15

``` r
#Variance
var(cars$speed)
```

    ## [1] 27.95918

``` r
#Standard Deviation
sd(cars$speed)
```

    ## [1] 5.287644

``` r
#Interquartile Range
IQR(cars$speed)
```

    ## [1] 7

``` r
#Min and Max
min(cars$speed)
```

    ## [1] 4

``` r
max(cars$speed)
```

    ## [1] 25

``` r
#Range
max(cars$speed)-min(cars$speed)
```

    ## [1] 21

``` r
#1st Quantile
quantile(cars$speed,.25)
```

    ## 25% 
    ##  12

``` r
#3rd Quantile
quantile(cars$speed,.75)
```

    ## 75% 
    ##  19

``` r
#Summary
summary(cars$speed)
```

    ##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
    ##     4.0    12.0    15.0    15.4    19.0    25.0

## Create plots

Create plots and modify the title and axis of a histgram using hist()

``` r
#Histogram
hist(cars$speed)
```

![](descriptive_statistics_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

``` r
#Histogram modify title
hist(cars$speed, main="Speed and Stopping Distance of Cars")
```

![](descriptive_statistics_files/figure-gfm/unnamed-chunk-2-2.png)<!-- -->

``` r
#Histogram modify x-axis
hist(cars$speed, xlab="Speed(mph)")
```

![](descriptive_statistics_files/figure-gfm/unnamed-chunk-2-3.png)<!-- -->

``` r
#Histogram modify title 
hist(cars$speed, xlab="Speed(mph)", main="Speed and Stopping Distance of Cars")
```

![](descriptive_statistics_files/figure-gfm/unnamed-chunk-2-4.png)<!-- -->
