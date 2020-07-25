---
bibliography: inst/bibliography.bib
---

# rientation: a sequential Monte Carlo approach to estimating orientation from inertial sensors in R

<!-- badges: start -->
<!-- badges: end -->


## Installation

`rientation` is not currently available on CRAN. You can install this package using:

``` r
#install.packages("devtools") # if devtools is not installed
devtools::install_github("shreeramsenthi/rientation")
```

## Overview

`rientation` is a package for estimating orientation from inertial sensor data using a sequential Monte Carlo smoother in R.
This differs from other available packages that estimate orientation from similar datasets in that it makes use of the entire sequence of inertial sensor readings to estimate the orientation of the sensor at each time point, rather than only using past and present measurements.
In addition, this package streamlines estimating sensor bias and sensitivity along each axis and for each sensor modality (gyroscope, accelerometer, magnetometer) from the data if the sensors have not been characterized.
The algorithm is adapted from @yang2018, with parameter estimation adapted from @liu2001, and smoothing adapted from @godsill2004.

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(rientation)
## basic example code
```

## References
