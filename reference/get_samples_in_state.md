# Get samples (finest grained data) for a state.

Get samples (finest grained data) for a state.

## Usage

``` r
get_samples_in_state(
  bdate = bdate,
  edate = edate,
  state.fips = state.fips,
  param = param,
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

- state.fips:

  State FIPS code. Use get_state_fips() if unsure.

- param:

  Pollutant parameter that site is measuring.

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

API response containing sample measurements in a state.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20160101"
edate <- "20160102"
state.fips <- "15"
param <- "42401"
result <- get_samples_in_state(bdate = bdate, 
                               edate = edate, 
                               param = param, 
                               state.fips = state.fips)
result$Data
} # }
```
