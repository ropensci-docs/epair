# Internal function to perform geospatial lookup by monitoring agency.

Internal function to perform geospatial lookup by monitoring agency.

## Usage

``` r
lookup_by_ma(
  endpoint,
  bdate,
  edate,
  param,
  agency,
  cached = TRUE,
  cache_directory = "/cache"
)
```

## Arguments

- endpoint:

  Base url to make call.

- bdate:

  Beginning date to check. Year, month, day format.

- edate:

  Ending date to check. Year, month, day format.

- param:

  Pollutant parameter that site is measuring.

- agency:

  The monitoring agency.

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20201231"
param <- "44201"
agency <- "0013"
result <- lookup_by_ma(QA_APE, bdate, edate, param, agency)
result$Data
} # }
```
