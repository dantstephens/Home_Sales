# Home_Sales
Completed by Daniel Stephens

## Overview of this project

This project demonstrates the use of PySpark SQL to read and query dataframes using SQL. Additionally, we optimize the data by caching the table, as well as paritioning into a parquet file, to compare query performance against un-optimized tables. 

## Home_Sales.ipynb

In this notebook, the dataset is loaded from a CSV file into a data frame using Spark. We then create a temporary table from the data frame and perform multiple SQL queries using Spark SQL. Next, to optimize run time for our queries, we cache the table and then re-run the last query to compare run times. After confirming improved run times, we partition the table into a Parquet file, create another temporary view from the Parquet file, and then re-run the last query to see if we get any performance gains. Lastly, we finish up by uncaching the table. 

## Running the app

-This notebook is set up to run from Google Colab
-The CSV file is read from an S3 bucket, so the notebook file can be run from any location
-When running the notebook from Colab, the Spark version number on line 3 of the first cell must be set to the latest version('spark-3.4.2' as of 3/6/2024). The latest distro can be found at from http://www.apache.org/dist/spark/ 
