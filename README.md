# Home_Sales
Completed by Daniel Stephens

## Overview of this project

This project demonstrates the use of PySpark SQL to read and query dataframes using SQL. Additionally, we optimize the data by caching the table, as well as paritioning into a parquet file, to compare query performance against un-optimized tables. 

## home_sales.ipynb

In this notebook, the dataset is loaded from a CSV file into a data frame using Spark. We then create a temporary table from the data frame and perform multiple SQL queries using Spark SQL. Next, to optimize run time for our queries, we cache the table and then re-run the last query to compare run times. After confirming improved run times, we partition the table into a Parquet file, create another temporary view from the Parquet file, and then re-run the last query to see if we get any performance gains. Lastly, we finish up by uncaching the table. 
