# Get annual summary data at a measurement site.

Get annual summary data at a measurement site.

## Usage

``` r
get_annual_summary_in_site(
  bdate,
  edate,
  param,
  state.fips,
  county,
  site,
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

- param:

  Pollutant parameter that site is measuring.

- state.fips:

  State FIPS code. Use get_state_fips() if unsure.

- county:

  County code. Use get_counties_in_state() if unsure.

- site:

  Measurement site code. Use get_sites_by_county() if unsure.

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing annual summary data for a site.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20170618"
edate <- "20170618"
state.fips <- "37"
county <- "183"
site <- "0014"
param <- "44201"
result <- get_annual_summary_in_site(bdate,
                                     edate,
                                     param,
                                     state.fips,
                                     county,
                                     site)
result$Data
} # }
```
