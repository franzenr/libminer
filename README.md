
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->
<!-- badges: end -->

The goal of libminer is to is to provide an overview of your R library
setup. This is a toy package created as part of the Fundamentals of
Package Development workshop given at Posit::conf(2023)

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("franzenr/libminer")
```

## Example

To get a count of the total number of installed packages in each of your
librarires, use `lib_summary()`. Including the optional `sizes = TRUE`
argument will also return the size of each library.

``` r
library(libminer)
## basic example code

lib_summary()
#>                                                                                         Library
#> 1                         /Library/Frameworks/R.framework/Versions/4.3-x86_64/Resources/library
#> 2 /private/var/folders/tw/9kctjvks4_n89wkzlx8xr001bj69l_/T/RtmpUgo71t/temp_libpath159742ba0d485
#>   n_packages
#> 1        126
#> 2          1
# specify sizes = TRUE
lib_summary(sizes = TRUE)
#>                                                                                         Library
#> 1                         /Library/Frameworks/R.framework/Versions/4.3-x86_64/Resources/library
#> 2 /private/var/folders/tw/9kctjvks4_n89wkzlx8xr001bj69l_/T/RtmpUgo71t/temp_libpath159742ba0d485
#>   n_packages lib_size
#> 1        126     6996
#> 2          1     6996
```
