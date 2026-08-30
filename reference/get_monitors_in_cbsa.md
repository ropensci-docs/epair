# Get monitors within a Core Based Statistical Area.

Get monitors within a Core Based Statistical Area.

## Usage

``` r
get_monitors_in_cbsa(
  bdate,
  edate,
  param,
  cbsa,
  cached = TRUE,
  cache_directory = "/cache"
)
```

## Arguments

- bdate:

  Beginning date to check. Year, month, day format.

- edate:

  Ending date to check. Year, month, day format.

- param:

  Pollutant parameter that site is measuring.

- cbsa:

  An encoding for a Core Base Statiscal Area. If unsure, use
  get_cbsas().

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Value

API response containing operational information about the monitor.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20200102"
cbsa <- "16740"
param <- "42401"
result <- get_monitors_in_cbsa(bdate, edate, param, cbsa)
result$Data
} # }
```
