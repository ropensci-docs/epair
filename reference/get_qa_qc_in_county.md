# Get quality assurance annual one point quality control data in a county.

Get quality assurance annual one point quality control data in a county.

## Usage

``` r
get_qa_qc_in_county(
  bdate,
  edate,
  state.fips,
  county,
  param,
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

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Value

API response containing operational information about the quality
assurance one point quality control data.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20170101"
edate <- "20171231"
state.fips <- "01"
county <- "003"
param <- "44201"
result <- get_qa_qc_in_county(bdate, edate, state.fips, county, param)
result$Data
} # }
```
