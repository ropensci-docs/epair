# Replace every string entry in a list

Replace every string entry in a list

## Usage

``` r
list.string.replacer(entry.list, pattern, replacement)
```

## Arguments

- entry.list:

  List containing character entries

- pattern:

  Pattern to replace

- replacement:

  Replacement for entries following the pattern

## Value

A list with entries matching the pattern replaced by replacement

## Examples

``` r
services <- list("\t Some text from the table")
services <- epair:::list.string.replacer(services, "\t", "")
services
#> [[1]]
#> [1] " Some text from the table"
#> 
```
