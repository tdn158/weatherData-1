# Install 

To install the development version of weatherData from github, use the **devtools** package.

```r
install.packages("devtools")
library("devtools")
install_github("weatherData", "Ram-N")
```

Load the library
```r
library(weatherData)
```


Windows users must also first install
[Rtools](http://cran.rstudio.com/bin/windows/Rtools/).

## Suggestions

Suggestions are welcome! If you would have a particular need for weather data,
let me know what changes you'd like to see in the package. If you find bugs, please do report it. Fetching data from the web can be fragile.
Submit an Issue.

# How to Use this package

## Examples 


```r
library(weatherData)
IsStationDataAvailable("SFO", "2010-10-29", "2013-01-12")
```

The command above will see if weather data is available for the Airport supplied ("SFO") for the two end dates supplied: for the 20th Oct 2010 and for Jan 12th 2013 in this case.

This command is useful for a quick check, before invoking `getDateRangeWeather`

```r
data(London2013)
```
This is a data frame of Ambient temperature data, extracted
from Weather Undergound. Each row has two entries
(columns). The Timestamp (YYYY-MM-DD HH:MM:SS) and the
TemperatureF (in degrees F) 




