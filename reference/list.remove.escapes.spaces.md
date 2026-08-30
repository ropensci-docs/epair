# Remove tabs, new lines, and empty spaces from entries in a list

Remove tabs, new lines, and empty spaces from entries in a list

## Usage

``` r
list.remove.escapes.spaces(a.list)
```

## Arguments

- a.list:

  List to remove entries from.

## Value

A list without tabs, new lines, and empty spaces

## Examples

``` r
service <- c("Sign up")
description <- c("Email will\r\n\t\t\t\t\t\t\t be sent to the registered
address from aqsdatamart@epa.gov.")

og_list <- list("service" = service, "description" = description)
clean <- epair:::remove.escapes.spaces(og_list)
clean
#>   service
#> 1 Sign up
#>                                                               description
#> 1 Email will be sent to the registered\naddress from aqsdatamart@epa.gov.
```
