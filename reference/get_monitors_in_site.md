# Get all monitors at a site.

Get all monitors at a site.

## Usage

``` r
get_monitors_in_site(
  bdate,
  edate,
  state.fips,
  county,
  param,
  site,
  cached = TRUE,
  cache_directory = "/cache"
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

- param:

  Pollutant parameter that site is measuring.

- site:

  Measurement site code. Use get_sites_by_county() if unsure.

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
state.fips <- "37"
county <- "001"
param <- "42401"
site <- "001"
result <- get_monitors_in_site(bdate, edate, state.fips, county, param, site)
result$Data
} # } 
```
