# genHz-rules
Keeping track of micro-correlation decisions, related to the functional grouping of genetic soil horizon designations.


Some options:
  * .R files, one per soil series concept
  * pedon records in NASIS via "component layer ID"
  * R lists, all in one super-list
  * a list of R S3/S4 objects
  * JSON representation that can be converted to a named list in R via `jsonlite` functions
  * files associated with the [`soilReports` package](https://github.com/ncss-tech/soilReports)
  * ???
  

## JSON

### Encode
```r
library(jsonlite)
toJSON(gen.hz.rules, pretty = TRUE)
```

### Decode
```r
library(jsonlite)
x <- 
ghl <- fromJSON(x)
```

