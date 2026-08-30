# Get quality assurance annual performance evaluations for a primary quality assurance organization.

Get quality assurance annual performance evaluations for a primary
quality assurance organization.

## Usage

``` r
get_qa_ape_in_pqao(
  bdate,
  edate,
  param,
  pqao,
  cached = TRUE,
  cache_directory = "/cache"
)
```

## Arguments

- bdate:

  Beginning date to check. Year, month, day format.

- edate:

  Ending date to check. Year, month, day format.

- param:

  Pollutant parameter that site is measuring.

- pqao:

  An encoding for a primary quality assurance organization. If unsure,
  use get_all_pqaos().

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Value

API response containing operational information about the quality
assurance annual performance evaluations.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20170101"
edate <- "20171231"
pqao <- "0013"
param <- "44201"
result <- get_qa_ape_in_pqao(bdate, edate, param, pqao)
result$Data
} # }
```
