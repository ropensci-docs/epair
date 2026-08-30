# Get quality assurance PEP audit data for a primary quality assurance organization.

Get quality assurance PEP audit data for a primary quality assurance
organization.

## Usage

``` r
get_qa_pep_in_pqao(
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
assurance PEP audit data.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20180101"
edate <- "20181231"
param <- "88101"
pqao <- "0013"
result <- get_qa_pep_in_pqao(bdate, edate, param, pqao)
result$Data
} # }
```
