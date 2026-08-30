# Get quarterly summary data in a bounding box (lat, long).

Get quarterly summary data in a bounding box (lat, long).

## Usage

``` r
get_quarterly_summary_in_bbox(
  bdate,
  edate,
  param,
  minlat,
  maxlat,
  minlong,
  maxlong,
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

- minlat:

  Minimum latitude coordinate.

- maxlat:

  Maximum latitude coordinate.

- minlong:

  Minimum longitude coordinate.

- maxlong:

  Maximum longitude coordinate.

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing quarterly summary data in a bounding box.

## Examples

``` r
if (FALSE) { # \dontrun{
bdate <- "20200101"
edate <- "20200102"
param <- "42401"
minlat <- 33.3
maxlat <- 33.6
minlong <- -87
maxlong <- -86.7
result <- get_quarterly_summary_in_bbox(bdate,
                                        edate,
                                        param,
                                        minlat,
                                        maxlat,
                                        minlong,
                                        maxlong)
result$Data
} # }
```
