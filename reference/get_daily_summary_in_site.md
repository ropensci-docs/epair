# Returns data summarized by day at measurement site level.

Returns data summarized by day at measurement site level.

## Usage

``` r
get_daily_summary_in_site(
  bdate,
  edate,
  state.fips,
  county,
  site,
  param,
  cached = TRUE,
  cache_directory = "/cache",
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

- county:

  County code. Use get_counties_in_state() if unsure.

- site:

  Measurement site code. Use get_sites_by_county() if unsure.

- param:

  Pollutant parameter that site is measuring.

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

- cbdate:

  Change begin date. (Optional)

- cedate:

  Change end date. (Optional)

## Value

API response containing daily data.

## Examples

``` r
if (FALSE) { # \dontrun{
param <- 44201
bdate <- 20170618
edate <- 20170618
state <- 37
county <- 183
site <- 0014
result <- get_daily_summary_in_site(bdate,
                                    edate,
                                    state,
                                    county,
                                    site,
                                    param)
result$Data
} # }
```
