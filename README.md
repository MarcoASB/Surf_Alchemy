# Surfs Up! :ocean: :palm_tree: :volcano:
## Climate Analysis for a holiday vacation in Honolulu, Hawaii! :hibiscus:

![surfs-up.png](surfs-up.png)

## Climate Analysis and Exploration

* Basic climate analysis and data exploration of the climate database with `Python` and `SQLAlchemy`.  
* Choose a start date and end date for the trip. Approximately 3-15 days total.
* Use SQLAlchemy `create_engine` to connect to the sqlite database.
* Use SQLAlchemy `automap_base()` to reflect tables into classes and save a reference to those classes called `Station` and `Measurement`.

### Precipitation Analysis

* Design a query to retrieve the last 12 months of precipitation data.
* Select `date` and `prcp` values.
* Load the query results into a Pandas DataFrame.
* Plot the results using the DataFrame `plot` method.

### Station Analysis

* Calculate the total number of stations.
* Find the most active stations.
* Design a query to retrieve the last 12 months of temperature observation data (tobs) of the most active station

### Temperature Analysis
* Create a function that takes two arguments: start date and end date in the format `%Y-%m-%d` and return the minimum, average, and maximum temperatures for that range of dates.
* Use the function to calculate the min, avg, and max temperatures for the trip using the matching dates from the previous year 
    * i.e., using "2017-01-01" if the trip start date was "2018-01-01".
* Plot the min, avg, and max temperature from your previous query as a bar chart.
  * Use the average temperature as the bar height.
  * Use the peak-to-peak (tmax-tmin) value as the y error bar (yerr).
  
### Daily Rainfall Average.

* Calculate the rainfall per weather station using the previous year's matching dates.
* Calculate the daily normals. (Normals are the averages for the min, avg, and max temperatures.)
* Create a function that will calculate the daily normals for a specific date using all historic tobs that match that date string. 
    * The date string will be in the format `%m-%d`.
* Create a list of dates for the trip. 
* Use the function to calculate the normals for each date string and append the results to a list.
* Load the list of daily normals into a Pandas DataFrame and set the index equal to the date.
* Plot an area plot (`stacked=False`) for the daily normals.
