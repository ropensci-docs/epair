# Make the first call when forming a query.

Make the first call when forming a query.

## Usage

``` r
create.base.call(endpoint)
```

## Arguments

- endpoint:

  Endpoint for forming a query. See ENDPOINTS for all available
  endpoints. See SERVICES if you know the service but not the endpoint.

## Value

A URL string containing authentication for the call.

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- "list/states"
call <- epair:::create.base.call(endpoint)
call
} # }
```
