# Perform call and maintain JSON Lite structure

Perform call and maintain JSON Lite structure

## Usage

``` r
place.call.raw(url)
```

## Arguments

- url:

  URL following structure from EPA API

## Value

Results of data request in JSON format

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- 'list/states'
call <- create.base.call(endpoint)
raw.call <- place.call.raw(call)
raw.call
} # }
```
