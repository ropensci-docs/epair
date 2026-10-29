# Transpose a data frame

Transpose a data frame

## Usage

``` r
get.transpose(df)
```

## Arguments

- df:

  Data frame to be transposed

## Value

The transposed data frame. First variable entries become column names.

## Examples

``` r
service <- c("Sign up")
description <- c("Email will\r\n\t\t\t\t\t\t\t be sent to the registered 
address from aqsdatamart@epa.gov.")
df <- data.frame(service, description)
t.df <- epair:::get.transpose(df)
t.df
#>                                                                                                Sign up
#> service                                                                                        Sign up
#> description Email will\r\n\t\t\t\t\t\t\t be sent to the registered \naddress from aqsdatamart@epa.gov.
```
