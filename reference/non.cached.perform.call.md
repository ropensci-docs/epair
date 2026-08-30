# Perform call and convert data into list

Perform call and convert data into list

## Usage

``` r
non.cached.perform.call(endpoint, variables = list())
```

## Arguments

- endpoint:

  An endpoint from the available EPA API endpoints

- variables:

  A list of variables or a single variable to filter the EPA API
  endpoint.

## Value

A list containing requested data

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- 'list/states'
result <- non.cached.perform.call(endpoint)
} # }
```
