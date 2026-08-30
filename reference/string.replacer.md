# Replace all characters entries in data frame

Replace all characters entries in data frame

## Usage

``` r
string.replacer(df, pattern, replacement)
```

## Arguments

- df:

  Data frame containing character entries

- pattern:

  Pattern to use for matching

- replacement:

  Replacement of entries matching pattern

## Value

A data frame with entries following the pattern being replaced by
replacement

## Examples

``` r
df <- data.frame(c("1", "2", "3", "4"))
modified.df <- epair:::string.replacer(df, "1", "One")
modified.df
#>   c..1....2....3....4..
#> 1                   One
#> 2                     2
#> 3                     3
#> 4                     4
```
