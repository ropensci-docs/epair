# Add variables to a query

Add variables to a query

## Usage

``` r
add.variables(query, variables)
```

## Arguments

- query:

  A URL containing authentication for the EPA API site.

- variables:

  A list of variables. Each variable should be declared with the
  appropriate name. Consult VARIABLE.TYPES for the right names.

## Value

A URL consisting of query + variables.

## Examples

``` r
if (FALSE) { # \dontrun{
endpoint <- "dailyData/byState"
variable.list <- list("state" = '37', 
                      "bdate" = '20200101', 
                      "edate" = '20200102', 
                      "param" = '44201')
call <- epair::create.base.call(endpoint)
call <- add.variables(call, variable.list)
call
} # }
```
