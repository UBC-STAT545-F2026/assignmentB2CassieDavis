
<!-- README.md is generated from README.Rmd. Please edit that file -->

# assignmentB2CassieDavis

<!-- badges: start -->

<!-- badges: end -->

assignmentB2CassieDavis is a package that has a function called
count_all_missing_by_group() that counts the number of missing values in
a dataset. It groups observations by a selected variable and calculates
how many missing variables there are in each column for each group,
making it easier to identify missing data patterns across groups.

## Installation

You can install the development version of assignmentB2CassieDavis from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github(
  "UBC-STAT545-F2026/assignmentB2CassieDavis",
  ref = "0.1.0")
```

## Example

This example uses the built-in `airquality` dataset to count missing
values in each column, grouped by month.

``` r
library(assignmentB2CassieDavis)

count_all_missing_by_group(airquality, Month)
#> # A tibble: 5 × 6
#>   Month Ozone Solar.R  Wind  Temp   Day
#>   <int> <int>   <int> <int> <int> <int>
#> 1     5     5       4     0     0     0
#> 2     6    21       0     0     0     0
#> 3     7     5       0     0     0     0
#> 4     8     5       3     0     0     0
#> 5     9     1       0     0     0     0
```
