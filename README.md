# TimeSeriesDataSets

Repo containing csv versions of canonical data sets used for benchmarking and analyzing time series analysis and forecasting models. 
Intended to be easily callable from an ML script or Jupyter notebook and used for tutorial or pedagogical purposes. 

## Example of loading csv into script directly from repo:

```
import pandas as pd
air_passengers_url = ("https://github.com/SkanderHn/TimeSeriesDataSets/raw/master/data/air_passengers.csv")
df = pd.read_csv(air_passengers_url)
```
Make sure that you are using the path with: 
```"https://github.com/SkanderHn/TimeSeriesDataSets/raw/master/data/{file name}"```
not
```"https://github.com/SkanderHn/TimeSeriesDataSets/blob/master/data/{file name}"```

If you use the url with "blob", you will get a Pandas parsing error. 

## Air Passengers data set:
**File name:** air_passengers.csv   
**Frequency:** monthly.    
**Metric:** Total number of international air passengers.    
**Duration:** 1949-01 through 1960-12 / 12 years.      
**Number of series:** 1.   
**Number of data points:** 144.   
**Missing values:** No.    
**Reference:** *Box and Jenkins (1976): Times Series Analysis: Forecasting and Control*   
**Comments:** The "Iris data set" of time series forecasting and analysis. Clear linear trend and a multiplicative seasonal component - good for "sanity checking" a forecasting method.    

## Australian Tourism data set:
**File name:** australian_tourism.csv     
**Frequency:** Quarterly.     
**Metric:** Number of nights spent away from home (e.g. hotel visits) in Australia, aggregated up to 20 geogrephical subdivisions. Geographical subdivisions are obtained by first considering each state in Australia seperately and then further dividing each state in smaller areas of interest (e.g. Metro, North Coast, South Coast, etc...). See [here](https://otexts.com/fpp2/hts.html) for additional details.        
**Duration:** 1998-01 through 2016-10 / 19 years.    
**Number of series:** 20.     
**Number of data points:** 1520 time series values + 20 static feature values     
**Missing values:** No.        
**Reference:** *Athanasopoulos, G., & Hyndman, R. J. (2008). Modelling and forecasting Australian domestic tourism. Tourism 
Management, 29.*      
**Comments:** Canonical example of grouped/hierarchical time series with static features (in this case, the georaphical location of each times series).    

