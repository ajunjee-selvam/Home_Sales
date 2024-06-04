# Home_Sales

The purpose of this assignment is to use SparkSQL to determine key metrics from home sales data. This project involved using Spark to create temporary views, partition data, cache and uncache a temporary table, and verify that the table was uncached upon completion. 

## Dependencies and Packages
The following dependencies and packages are required for the execution of this project:
- installation of JAVA and spark-3.5.1
- os
- findspark
- pyspark.sql; SparkSession
- time
- pyspark; SparkFiles

## Steps
The following steps were executed to prepare the views for deriving key metrics and uncaching the temporary views upon completion:
1) Install Spark and Java, and import the necessary lbraries
2) Start a SparkSession
3) Read the AWS S3 bucket into a dataframe
4) Create a temporary view of the dataframe
5) Determine the key metrics using sql filtering
6) Cache the temporary table and check if it was cached
7) Rerun the last query to see how the runtime changes
8) Partition by the "date_built" field on the formatted parquet home sales data
9) Create a temporary view for this dataframe
10) Rerun the last query using the parquest dataframe and see how the runtime changes
11) Uncache the temporary table
12) Check to see if the table has been uncached
