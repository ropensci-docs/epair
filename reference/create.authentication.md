# Generate the string authentication needed for EPA API

Generate the string authentication needed for EPA API

## Usage

``` r
create.authentication(email, key)
```

## Arguments

- email:

  Email registered with EPA API

- key:

  Key obtained from EPA API. Register your email for a key here
  https://aqs.epa.gov/aqsweb/documents/data_api.html#signup.

## Value

A string with authentication info. It looks like
'&email=user_email&key=user_key'.

## Examples

``` r
auth <- create.authentication("myemail@domain.com", "myapikey")
auth
#> [1] "&email=myemail@domain.com&key=myapikey"
```
