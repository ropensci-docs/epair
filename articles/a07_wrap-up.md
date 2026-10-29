# Summary

Now you know how to make calls! The general template for making a call
(after making sure authentication is set up) is as follows.

## Option 1: User friendly functions

1.  Make the call with the appropriate `get` function for the service.

``` r

result <- get_state_fips()
```

2.  If the call requires a single variable, declare the variable with
    the variable name and pass it as an argument, or directly pass it as
    an argument.

``` r

result <- get_counties_in_state(state.fips = 'value')
```

3.  If the call requires multiple variables, pass each variable as it’s
    corresponding argument.

``` r

result <- get_annual_summary_in_state(bdate = "value.one",
                                      edate = "value.two",
                                      state.fips = "value.three",
                                      param = "value.four")
```

## Option 2: Manually placing the call

1.  Determine an endpoint for your service (possibly with the `services`
    object).

``` r

endpoint <- 'APIEndpoint'
```

2.  Make the call with
    [`perform.call()`](https://docs.ropensci.org/epair/reference/perform.call.md).

``` r

result <- perform.call(endpoint)
```

3.  If the call requires a single variable, declare the variable with
    the API variable name and pass it in as a second argument in
    [`perform.call()`](https://docs.ropensci.org/epair/reference/perform.call.md).

``` r

variable <- "value"
result <- perform.call(endpoint, variable)
```

Or, specify the name of the API variable in the third argument.

``` r

variable.code <- "value"
result <- perform.call(endpoint, variable.code, name = "API variable name")
```

4.  If the call requires multiple variables, make a list and pass it in
    as a second argument in
    [`perform.call()`](https://docs.ropensci.org/epair/reference/perform.call.md).

``` r

variables <- list(variable.one = "value.one",
                  variable.two = "value.two",
                  variable.three = "value.three")
result <- perform.call(endpoint, variables)
```

Or, specify the names of parameter codes in the second argument.

``` r

variables <- list("value.one", "value.two", "value.three")
result <- perform.call(endpoint, 
                       variables,
                       name = list("variable.one", "variable.two", "variable.three"))
```
