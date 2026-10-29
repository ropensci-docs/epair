# Get samples (finest grained data) for a Core Based Statistical Area.

Get samples (finest grained data) for a Core Based Statistical Area.

## Usage

``` r
get_samples_in_cbsa(
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

  Change begin date. (Optional)

- cedate:

  Change end date. (Optional)

## Value

API response containing sample measurements in a CBSA.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20200102"
cbsa <- "16740"
param <- "42401"
result <- get_samples_in_cbsa(bdate, edate, cbsa, param)
result$Data
} # }
```
