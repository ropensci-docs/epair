# Internal function to perform geospatial lookup by bounding box (lat, long).

Internal function to perform geospatial lookup by bounding box (lat,
long).

## Usage

``` r
lookup_by_bbox(
  endpoint,
  bdate,
  edate,
  param,
  minlat,
  maxlat,
  minlong,
  maxlong,
  cached = TRUE,
  cache_directory = "/cache",
  duration = NULL,
  cbdate = NULL,
  cedate = NULL
)
```

## Arguments

- endpoint:

  Base url to make call.

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

- duration:

  The 1-character AQS sample duration code. (Optional)

- cbdate:

  Beginning date of last change to DB. (Optional)

- cedate:

  Ending date of last change to DB. (Optional)

## Value

API response containing bbox bounded data.

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
result <- lookup_by_bbox(MONITORS, bdate, 
                                   edate, 
                                   param, 
                                   minlat, 
                                   maxlat, 
                                   minlong, 
                                   maxlong)
result$Data
} # }
```
