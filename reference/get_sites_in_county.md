# Get all measurement sites within a county.

Get all measurement sites within a county.

## Usage

``` r
get_sites_in_county(state.fips, county.code)
```

## Arguments

- state.fips:

  A state FIPS code. Use get_state_fips() to find the appropriate FIPS
  code.

- county.code:

  A county code. Use get_counties_in_state() to find the appropriate
  code for a given county.

## Value

API response containing all measurement sites within a given county.

## Examples

``` r
if (FALSE) { # \dontrun{
state <- "37"
county.code <- "001"
measurement.sites <- get_sites_in_county(state, county.code)
measurement.sites$Data 
} # }
```
