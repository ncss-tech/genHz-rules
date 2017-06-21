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
# get an example, results in a list called "gen.hz.rules"
source('https://raw.githubusercontent.com/ncss-tech/genHz-rules/master/named-list-example.R')
# convert to JSON for editing, ...?
toJSON(gen.hz.rules, pretty = TRUE)
```

### Decode
```r
library(jsonlite)
# convert JSON representation to named list
ghl <- fromJSON('https://raw.githubusercontent.com/ncss-tech/genHz-rules/master/example.json')
```

