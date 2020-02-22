# TimeSeriesDataSets

Repo containing csv versions of canonical data sets used for benchmarking and analyzing time series analysis and forecasting models. 
Intended to be easily callable from an ML script or Jupyter notebook and used for tutorial or pedagogical purposes. 

## Air Passengers data set:
Frequency: monthly. 
Metric: Total number of international air passengers. 
Duration: 1949-01 through 1960-12 / 12 years. 
Number of series: 1. 
Number of data points: 144. 
Missing values: No.  
Reference: *Box and Jenkins (1976): Times Series Analysis: Forecasting and Control*   
Comments: The "Iris data set" of time series forecasting and analysis.   

## Australian Tourism data set:
Frequency: Quarterly.  
Metric: Number of nights spent away from home (e.g. hotel visits) in Australia, aggregated up to 20 geogrephical subdivisions. 
Geographical subdivisions are obtained by first considering each state in Australia seperately and then further dividing each state in smaller areas of interest (e.g. Metro, North Coast, South Coast, etc...). See [here](https://otexts.com/fpp2/hts.html) for additional details.      
Duration: 1998-01 through 2016-10 / 19 years. 
Number of series: 20. 
Number of data points: 1520. 
Missing values: No.    
Reference: *Athanasopoulos, G., & Hyndman, R. J. (2008). Modelling and forecasting Australian domestic tourism. Tourism 
Management, 29.*  
Comments: Canonical example of grouped/hierarchical time series with static features (in this case, the georaphical location of each times series). 

