# Movies ETL

## Overview of Analysis
The purpose of this challenge is to create an automated pipline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. This automated pipeline is a process known as 'Extract, Transform and Load" or ETL. The topic is movies from 1990 to 2018 and combining the information from 3 different resources.

## Resources
1. Python
2. jupyter notebook
3. PostgresSQL and pgAdmin
4. Data sources: 3 files
   1. wifkipedia-movies.json (sourced by wikipedia.com)
   2. movies_metatdata.csv (sourced by kaggle.com)
   3. ratings.cvs (sourced by MovieLens)
   
## Results of Analysis

The goal was to clean, merge, and export two new tables to a SQL database using python.  

### Verifying the data in PgAdmin

To verify the data was successfully imported into the database, two queries were run. 

__Movies Query__

The movie tbl code to update the SQL database replaced any matching 
data

![tbl](/resources/sql-movie-count.png)

__Ratings Query__

The rating tbl code to update the SQL database *appended* to the existing table, which explains why it is twice as large as the ratings.csv.  
![tbl](/resources/sql-ratings-count.png)


### Issues 

Please note, two of the data sources exceeded the file limits of GitHub, and are not included in this repo.
1. wifkipedia-movies.json (sourced by wikipedia.com)
2. ratings.cvs (sourced by MovieLens)
