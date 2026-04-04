
<!-- README.md is generated from README.Rmd. Please edit that file -->

[!IMPORTANT]
This is work in progress.
This repository is an attempt to make a standalone r-inla package so that it can be served from places like Posit Package Manager and potentially CRAN.
Current status:
- `inst` folder has a bunch of symlinks that probably can be avoided, currently these are copied over from the parent repo;
- an R file ('likelihood.R') is missing from the Collate: in DESCRIPTION;
- `tidyterra` and `inlabru` missing as dependencies when building vignettes;
- vignettes fail to build (trying on ubuntu 25.10, but there is no inla binary for that version).
- tests run but many fail `[ FAIL 10 | WARN 0 | SKIP 0 | PASS 20 ]`




# INLA

<!-- badges: start -->

[![R-CMD-check](https://github.com/discindo/newscatcheR/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/discindo/newscatcheR/actions/workflows/R-CMD-check.yaml)
![pkgdown](https://github.com/novica/rinla/workflows/pkgdown/badge.svg)
<!-- badges: end -->

The goal of INLA is to …

## Installation

You can install the development version of INLA like so:

``` r
# FILL THIS IN! HOW CAN PEOPLE INSTALL YOUR DEV PACKAGE?
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
#library(rinla)
## basic example code
```

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

``` r
summary(cars)
#>      speed           dist       
#>  Min.   : 4.0   Min.   :  2.00  
#>  1st Qu.:12.0   1st Qu.: 26.00  
#>  Median :15.0   Median : 36.00  
#>  Mean   :15.4   Mean   : 42.98  
#>  3rd Qu.:19.0   3rd Qu.: 56.00  
#>  Max.   :25.0   Max.   :120.00
```

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
