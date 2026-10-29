# Get quality assurance PEP audit data in a state.

Get quality assurance PEP audit data in a state.

## Usage

``` r
get_qa_pep_in_state(
  bdate,
  edate,
  state.fips,
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
assurance PEP audit data.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20180101"
edate <- "20181231"
state.fips <- "01"
param <- "88101"
result <- get_qa_pep_in_state(bdate, edate, state.fips, param)
result$Data
} # }
```
