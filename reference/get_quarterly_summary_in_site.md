# Returns data summaries by yearly quarter.

Returns data summaries by yearly quarter.

## Usage

``` r
get_quarterly_summary_in_site(
  bdate,
  edate,
  state.fips,
  county,
  param,
  site,
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

- param:

  Pollutant parameter that site is measuring.

- site:

  Measurement site code. Use get_sites_by_county() if unsure.

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing quarterly summary data at a site.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20200102"
state.fips <- "37"
county <- "001"
site <- "001"
param <- "42401"
result <- get_quarterly_summary_in_site(bdate, 
                                        edate, 
                                        state.fips, 
                                        county, 
                                        param, 
                                        site)
result$Data
} # }
```
