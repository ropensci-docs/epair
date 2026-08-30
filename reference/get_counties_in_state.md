# Get all counties within a state.

Get all counties within a state.

## Usage

``` r
get_counties_in_state(state.fips)
```

## Arguments

- state.fips:

  A state FIPS code. Use get_state_fips() to find the appropriate FIPS
  code.

## Value

API response containing all counties and county codes within a given
state.

## Examples

``` r
if (FALSE) { # \dontrun{
state <- "37"
counties.in.state <- get_state_fips(state)
counties.in.state$Data
} # }
```
