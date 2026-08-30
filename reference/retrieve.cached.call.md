# Retrieves memory of previously cached call.

Retrieves memory of previously cached call.

## Usage

``` r
retrieve.cached.call(endpoint, variables = list(), directory = "/cache")
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
endpoint <- 'list/states'
retrieve.cached.call(endpoint)
#> NULL
```
