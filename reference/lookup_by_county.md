# Internal function to perform geospatial lookup by county.

Internal function to perform geospatial lookup by county.

## Usage

``` r
lookup_by_county(
  endpoint,
  bdate,
  edate,
  state.fips,
  county,
  param,
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

- state.fips:

  State FIPS code. Use get_state_fips() if unsure.

- county:

  County code. Use get_counties_in_state() if unsure.

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

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing operational information about the monitor.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20200102"
state.fips <- "37"
county <- "001"
param <- "42401"
result <- lookup_by_county(MONITORS, bdate, edate, state.fips, county, param)
result$Data
} # }
```
