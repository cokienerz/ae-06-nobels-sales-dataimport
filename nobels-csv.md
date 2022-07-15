Nobel winners
================
Naomi Ekas

``` r
library(tidyverse)
```

Let’s first load the data:

``` r
nobel <- read_csv("data-raw/nobel.csv")
```

Then let’s split the data into two:

``` r
# stem laureates
nobel_stem <- nobel %>%
  filter(category %in% c("Physics", "Medicine", "Chemistry", "Economics"))

# non-steam laureates
nobel_nonstem <- nobel %>%
  filter(!category %in% c("Physics", "Medicine", "Chemistry", "Economics"))
```

And finally write out the data:

``` r
# add code for writing out the two data frames here
```
