
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ESPENAPI

<!-- badges: start -->

<!-- badges: end -->

The goal of ESPENAPI is to provide access to Neglected Tropical Diseases
(NTDs) data from the ESPEN portal and provide a minimum
visualisation/summary of the data. Instead of having to visit the ESPEN
portal to download the data, this R package allows the user to acquire
the data and process it directly from
R.

## Installation

<!-- You can install the released version of ESPENAPI from [CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("ESPENAPI")
```
-->

You can install the development version from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("olatunjijohnson/ESPENAPI", ref="main")
```

## Example

This is a basic example which shows how to download the STH data at site
level from Kenya for 2010.

``` r
library(ESPENAPI)
data  <- ESPENAPI::ESPEN_API_data(country="Kenya", disease="sth", level="sitelevel", start_year=2010, end_year=2010)
## basic example code
```

## Further improvements

1.  Allows user to only supply api\_key once and it saves into the
    environment

2.  Develop another function to download maps from ESPEN portal

3.  Develop dashboard to summarise the data
