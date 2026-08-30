# Shows contents of cache directory

Shows contents of cache directory

## Usage

``` r
list.cached.data(directory = "/cache")
```

## Arguments

- directory:

  Place inside user-level cache directory that was used to store the
  cached data previously. Default: "/cache".

## Value

Character vector of file names currently in cache directory.

## Examples

``` r
if (FALSE) { # \dontrun{ 
my.files <- list.cached.data()
my.files 
} # }
```
