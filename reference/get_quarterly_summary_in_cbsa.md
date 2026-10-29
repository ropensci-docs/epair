# Get quarterly summary data in a Core Based Statistical Area.

Get quarterly summary data in a Core Based Statistical Area.

## Usage

``` r
get_quarterly_summary_in_cbsa(
  bdate,
  edate,
  param,
  cbsa,
  cbdate = NULL,
  cedate = NULL
)
```

## Arguments

- bdate:

  Beginning date to check. Year, month, day format.

- edate:

  Ending date to check. Year, month, day format.

- param:

  Pollutant parameter that site is measuring.

- cbsa:

  An encoding for a Core Base Statiscal Area. If unsure, use
  get_cbsas().

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing quarterly summary data at the cbsa level.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20190101"
edate <- "20190601"
cbsa <- "16740"
param <- "42401"
result <- get_quarterly_summary_in_cbsa(bdate, 
                                        edate, 
                                        param, 
                                        cbsa)
result$Data
} # }
```
