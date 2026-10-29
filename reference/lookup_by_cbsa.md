# Internal function to perform geospatial lookup by Core Based Statistical Area.

Internal function to perform geospatial lookup by Core Based Statistical
Area.

## Usage

``` r
lookup_by_cbsa(
  endpoint,
  bdate,
  edate,
  param,
  cbsa,
  cached = TRUE,
  cache_directory = "/cache",
  duration = NULL,
  cbdate = NULL,
  cedate = NULL
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

- cbsa:

  An encoding for a Core Base Statiscal Area. If unsure, use
  get_cbsas().

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

- duration:

  The 1-character AQS sample duration code. (Optional)

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing data at the cbsa level.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20200102"
cbsa <- "16740"
param <- "42401"
result <- lookup_by_cbsa(MONITORS, bdate, edate, param, cbsa)
result$Data
} # }
```
