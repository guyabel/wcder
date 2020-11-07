
<!-- README.md is generated from README.Rmd. Please edit that file -->

# wcder

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/wcder)](https://CRAN.R-project.org/package=wcder)
<!-- badges: end -->

Download data from the [Wittgenstein Human Capital Data
Explorer](http://dataexplorer.wittgensteincentre.org/wcde-v2/) into R

## Installation

<!-- You can install the released version of wcder from [CRAN](https://CRAN.R-project.org) with: -->

<!-- ``` r -->

<!-- install.packages("wcder") -->

<!-- ``` -->

Install the developmental version with:

``` r
library(devtools)
install_github("guyabel/wcder")
```

## Example

Download data based on a measure, scenario and country code:

``` r
library(wcder)

# Not Run
# SSP2 tfr for Austria and Bulgaria
# wcde(measure = "tfr", country_code = c(40, 100))

# SSP2 tfr for Austria and United Kingdom (guessing the country codes)
# wcde(measure = "tfr", country_name = c("Austria", "UK"))

# SSP1 and SSP3 population by education for all countries
# library(dplyr)
# wic_locations %>%
#   filter(dim == "country") %>%
#   pull(isono) %>%
#   wcde(scenario = c(1, 3), measure = "epop", country_code = .)
```

<!-- What is special about using `README.Rmd` instead of just `README.md`? You can include R chunks like so: -->

<!-- ```{r cars} -->

<!-- summary(cars) -->

<!-- ``` -->

<!-- You'll still need to render `README.Rmd` regularly, to keep `README.md` up-to-date. -->

<!-- You can also embed plots, for example: -->

<!-- ```{r pressure, echo = FALSE} -->

<!-- plot(pressure) -->

<!-- ``` -->

<!-- In that case, don't forget to commit and push the resulting figure files, so they display on GitHub! -->