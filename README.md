![title_illustration](Output_Data/HurriPy_cartoon.jpg)

## Project 1 - Data Analysis &amp; Visualization Boot Camp - McCombs School of Business, University of Texas, USA

A group of world-renowned data scientists took upon themselves to analyze the correlations between cyclones and impacting factors.

### The study hopes to provide information regarding:

#### Question 1: How do we understand tropical storms, cyclones, and hurricanes?
**Data exploration**: Data was retrieved from the National Hurricane Center's website (https://www.nhc.noaa.gov/data/#hurdat)  
**Data Cleanup**: Data was scrubbed in Excel to assign a unique storm name, type and Julian to each of the 52k rows to understand onset and duration of each individual storm.
**Data Analysis**: The cleaned .csv data was imported into Jupyter Notebooks as Pandas DataFrames. Certain data types were converted from float to integer. Bob and Kevin shared a new approach on setting tick locations for the bar graph. We used:dropna to omit NaN data, drop to filter DataFrames, and groupby to cluster data by cyclone type and the corresponding decade
**Data Visualization**:A stacked bar graph to understand the split between named vs. unnamed cyclones since 1950
	                 A bar graph to plot the duration of named cyclones with the decades as tick location markers
	                 A scatter plot to plot the cyclone patterns by decade and their corresponding onset in terms of time of the year. We also calculated the regression between onset and years.

#### Question 2: What are the demographics of an area before and after a storm?
**Data exploration**: Data was retrieved using Census API for population, poverty count, and median home value for three zip codes per cyclone.  
**Data Cleanup**: Retrieved data in 2018 that was NaN and that data was dropped using drop.na. 2016 and 2018 dataframes were merged to create a new data frame.  
**Data Analysis/Data Visualization**: Bar graphs were used to analyze the comparison of 2016 and 2018 demographics to see if cyclones impacted population, poverty count, and median home value.

#### Question 3: Does a tropical storm effect the temperature on land?
**Data exploration**: Data was retrieved using NOAA API for weather stations in the landfall area of each hurricane.  
**Data Cleanup**: Retrieved data had "SNOW" column, which indicates snow precipitation measured in that weather station. That column was discarded from the dataset.  
**Data Analysis**: The maximum and minimum temperatures, precipitation from every station were grouped according to the dates - 5 days before and 6 days after the landfall.  
**Data Visualization**: Line plots were made for precipitation, maximum and minimum temperatures were built to see the changes in those parameters during hurricane landfall.


## Data sets used:
https://www.census.gov/  
https://www.nhc.noaa.gov/  
https://www.weather.gov/  
https://www.flhurricane.com/  

## API keys requested from:
Census | Google maps | NOAA

#### Presented on 2020.06.25
