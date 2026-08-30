# Get samples (finest grained data) for a county.

Get samples (finest grained data) for a county.

## Usage

``` r
get_samples_in_county(
  bdate,
  edate,
  state.fips,
  param,
  county,
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

- county:

  County code.

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
county <- "001"
param <- "42401"
result <- get_samples_in_county(bdate = bdate,
                                edate = edate,
                                param = param,
                                state.fips = state.fips,
                                county = county)
result$Data
} # } 
```
