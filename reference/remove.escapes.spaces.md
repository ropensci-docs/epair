# Remove tabs, new lines, and empty spaces from entries in a data frame

Remove tabs, new lines, and empty spaces from entries in a data frame

## Usage

``` r
remove.escapes.spaces(df)
```

## Arguments

- df:

  Data frame to remove tabs, new lines, and empty spaces from

## Value

Data frame without tabs, new lines, and empty spaces

## Examples

``` r
service <- c("Sign up")
description <- c("Email will\r\n\t\t\t\t\t\t\t be sent to the registered
address from aqsdatamart@epa.gov.")

og.df <- data.frame(service, description)
clean.df <- epair:::remove.escapes.spaces(og.df)
clean.df
#>   service
#> 1 Sign up
#>                                                               description
#> 1 Email will be sent to the registered\naddress from aqsdatamart@epa.gov.
```
