# Removes memory of cached perform.call data for specific parameters

Removes memory of cached perform.call data for specific parameters

## Usage

``` r
clear.cached(endpoint, variables = list(), directory = "/cache")
```

## Arguments

- endpoint:

  An endpoint from the available EPA API endpoints

- variables:

  A list of variables or a single variable to filter the EPA API
  endpoint.

- directory:

  Place inside user-level cache directory that was used to store the
  cached data previously. Default: "/cache".

## Value

TRUE if data was successfully forgotten, error message if cached data
was not found

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- 'list/states'
clear.cached(endpoint)
} # }
```
