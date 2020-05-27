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
