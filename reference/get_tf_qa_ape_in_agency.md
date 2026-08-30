# Get quality assurance annual performance evaluations for a monitoring agency in transaction format.

Get quality assurance annual performance evaluations for a monitoring
agency in transaction format.

## Usage

``` r
get_tf_qa_ape_in_agency(
  bdate,
  edate,
  param,
  agency,
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

- agency:

  The monitoring agency.

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Value

API response containing operational information about the quality
assurance annual performance evaluations in transaction format.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20170101"
edate <- "20171231"
param <- "44201"
agency <- "0013"
result <- get_tf_qa_ape_in_agency(bdate, 
                              edate, 
                              param, 
                              agency)
result$Data
} # }
```
