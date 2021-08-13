# Module-8-Movies-ETL


## Module Overview
In this module we learned how to do a ETL (extract, transform, load) a 3 step process for building a data pipeline.
* Step 1 is extracting and staging multiple datasources. This could be JSON, HTML, CSV, Kaggle, ECT
* Step 2 is transform the data. With the goal of creating as much structural consistancy as possible from our various datasets, we do this by applying: filtering, parsing, sorting, summarizing, and more in this step
* Step 3 is Loading, now that we have a consistant data structure. We put it our data target. 

Building a accurate data pipeline is important for a data analyst, ETL is a essential skill for any data analyst.

## Module Objectives
* Create an ETL pipeline, transform provided raw data into a SQL database
* Extract/Explore the data into python as dataframes. 
* Clean and transform with python
* Use regular expressions and Parse the data. Transform text to int
* Load to PostgreSQL




## Module Summary

### ETL

<img width="572" alt="Screen Shot 2021-08-13 at 10 45 46 AM" src="https://user-images.githubusercontent.com/83923903/129399018-94f73691-eabf-41cb-b83a-e543b8d8d679.png">

ETL is pretty straight forward process. We have data that currently existing throughout multiple places and they will need to be structured and cleaned up before we can begin to analyze it. ETL breaks it into three steps: Extract, Transform, and Load. ETL is great, because its versitile, it can be used for a simple one time data migration or used to handle complex on going real time data sources.

*Extract: We Extracted scaped wikipedia_movie.json and kaggle data located in ratings & Movie_Metadata csv's

*Transform: we used Python and Pandas to document, explore, and perform our data transformation

*Load: Load our Data into our postgresSQL 

## Challenge Overview

* Create and Automate ETL Data pipeline
* Extraction from multiple data sources
* Apply Iterative process: Inspect, Plan and execute
* Clean and Transform data in pandas with regualr expressions, and function.
* Load our new data into postgreSQL

## Challenge Objectives

* Step Load: Create a function to extract values into numeric. We call it parse_dollars.

<img width="727" alt="Screen Shot 2021-08-13 at 11 35 17 AM" src="https://user-images.githubusercontent.com/83923903/129403979-b79716fc-60ef-45b8-aff9-25a541cc20ac.png">

* Step Transform: We re-used code from our module 8 jupyter notebook. We kept all function performing the transformation steps. We did removing all redundant code. To see Pre and Post
Pre: Please reference challenge.ipynb file in repo
Post: Please reference Challenge.py file in repo

* Step Load: We can see extract_transform_wiki work by loading into PostgreSQL

<img width="722" alt="Screen Shot 2021-08-13 at 11 41 17 AM" src="https://user-images.githubusercontent.com/83923903/129404568-89fd11d5-d436-4d74-8d1e-1a1807576529.png">

*Here is the output on PostgreSQL, we can see all 32 columns successfully loaded. Our ETL works.

<img width="1561" alt="Screen Shot 2021-08-13 at 11 40 19 AM" src="https://user-images.githubusercontent.com/83923903/129404483-c6adaf63-15c1-4a05-a3e7-ca92b99af06d.png">

## Challenge Roadblock

I had an issue the ratings.csv file the data file is simply too large. I am thinking of practical solutions one involving divinding up the CSV into smaller multiple files. I can always just re-merge them with SQL. Perhaps this maybe a solution. 

