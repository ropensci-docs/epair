# Perform call and keep original result

Perform call and keep original result

## Usage

``` r
perform.call.raw(endpoint, variables = list())
```

## Arguments

- endpoint:

  An endpoint from the available EPA API endpoints

- variables:

  A list of variables or a single variable to filter the EPA API
  endpoint.

## Value

A list containing result from query to EPA API

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- 'list/states'
result <- perform.call.raw(endpoint)
} # }
```
