# Get all parameters available within a particular parameter class.

Get all parameters available within a particular parameter class.

## Usage

``` r
get_parameters_in_class(class)
```

## Arguments

- class:

  A type of pollutant. Find types of pollutants with
  get_parameter_classes().

## Value

API response containing parameters found within a class/group of like
parameters.

## Examples

``` r
if (FALSE) { # \dontrun{
class <- "AQI POLLUTANTS"
parameters <- get_parameters_in_class(class)
parameters$Data
} # }
```
