# Get samples (finest grained data) for a bounding box (lat, long).

Get samples (finest grained data) for a bounding box (lat, long).

## Usage

``` r
get_samples_in_bbox(
  bdate,
  edate,
  minlat,
  maxlat,
  minlong,
  maxlong,
  param,
  cached = TRUE,
  cache_directory = "/cache",
  duration = NULL,
  cbdate = NULL,
  cedate = NULL
)
```

## Arguments

- bdate:

  Beginning date to check. Year, month, day format.

- edate:

  Ending date to check. Year, month, day format.

- minlat:

  Minimum latitude coordinate.

- maxlat:

  Maximum latitude coordinate.

- minlong:

  Minimum longitude coordinate.

- maxlong:

  Maximum longitude coordinate.

- param:

  Pollutant parameter that site is measuring.

- cached:

  TRUE or FALSE specifying if the data from the call is to be cached.
  Default: TRUE. (Optional)

- cache_directory:

  Place inside user-level cache directory to store the cached data.
  Default: "/cache". (Optional)

- duration:

  The 1-character AQS sample duration code. (Optional)

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

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
result <- get_samples_in_bbox(bdate = bdate,
                              edate = edate,
                              param = param,
                              minlat = minlat,
                              maxlat = maxlat,
                              minlong = minlong,
                              maxlong = maxlong)
result$Data
} # }
```
