# Installation

## How to install and load epair

### Directly from GitHub

Since it is on GitHub, installing `epair` in R with the `devtools`
package is straightforward.

``` r

library(devtools)
devtools::install_github("GLOrozcoM/epair")
library(epair)
```

### After downloading package files

An alternative is to download the epair files on to your computer from
GitHub. You can download them
[here](https://docs.ropensci.org/epair/articles/GLOrozcoM/epair). After
navigating to the parent folder of the epair directory, you can use
`devtools`.

``` r

devtools::install("epair")
library(epair)
```
