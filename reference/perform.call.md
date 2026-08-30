# Cached version of the perform.call function

Cached version of the perform.call function

## Usage

``` r
perform.call(
  endpoint,
  variables = list(),
  cached = TRUE,
  cache_directory = "/cache"
)
```

## Arguments

- endpoint:

  An endpoint from the available EPA API endpoints

- variables:

  A list of variables or a single variable to filter the EPA API
  endpoint.

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE.

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache".

## Value

A list containing requested data

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- 'list/states'
result <- perform.call(endpoint)
} # }
```
