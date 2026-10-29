# Saves a new call that has not been previously cached yet.

Saves a new call that has not been previously cached yet.

## Usage

``` r
save.new.cached.call(endpoint, variables = list(), directory = "/cache")
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

A list containing requested data

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- 'list/states'
save.new.cached.call(endpoint)
} # }
```
