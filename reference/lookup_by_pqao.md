# Internal function to perform geospatial lookup by primary quality assurance organization.

Internal function to perform geospatial lookup by primary quality
assurance organization.

## Usage

``` r
lookup_by_pqao(
  endpoint,
  bdate,
  edate,
  param,
  pqao,
  cached = TRUE,
  cache_directory = "/cache"
)
```

## Arguments

- endpoint:

  Base url to make call.

- bdate:

  Beginning date to check. Year, month, day format.

- edate:

  Ending date to check. Year, month, day format.

- param:

  Pollutant parameter that site is measuring.

- pqao:

  An encoding for a Primary Quality Assurance Organization. If unsure,
  use get_all_pqaos().

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20201231"
param <- "44201"
pqao <- "0013"
result <- lookup_by_pqao(QA_APE, bdate, edate, param, pqao)
result$Data
} # }
```
