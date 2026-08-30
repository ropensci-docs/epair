# Get all monitoring sites within a bounding box (lat, long).

Get all monitoring sites within a bounding box (lat, long).

## Usage

``` r
get_monitors_in_bbox(
  bdate,
  edate,
  param,
  minlat,
  maxlat,
  minlong,
  maxlong,
  cached = TRUE,
  cache_directory = "/cache"
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

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

## Value

API response containing operational information about the monitor.

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
result <- get_monitors_in_bbox(bdate, 
                              edate, 
                              param, 
                              minlat, 
                              maxlat, 
                              minlong, 
                              maxlong)
result$Data
} # }
```
