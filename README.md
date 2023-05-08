# Final-Project
###### This is my final project for DS 2002. It outlines the business process of a movie rental business using the sakila database. The solution meets all stated requirments.

##### Requirements:
Your solution (database schema) needn’t be complex, but should meet the following requirements:
• Your solution must include a Date dimension to enable the analysis of the business process over various intervals of time (the code for creating this in MySQL has already been provided for you).
• Your solution must include at least 3 additional dimension tables
  1) dim_customer
  2) dim_staff
  3) dim_inventory

• Your solution must populate its dimensions using data originating from the following sources:

o A relational database like MySQL, Oracle or SQL Server ->  dim_inventory

o A NoSQL database like MongoDB, Redis, Cassandra or HBase ->  dim_customer

o A Cloud file system like Azure Data Lake, AWS S3 hosting file-base data (e.g., JSON, CSV) o An API that returns a message payload (e.g., JSON, CSV, text) optional ->  dim_staff

• Your solution must include at least 1 fact table that captures the business process transactions ->  fact_rentals

• Your solution must integrate datum of differing granularity (static and near real-time); i.e.,
implement Databricks structured streaming to integrate hot-path and cold-path data. -> this is implemented using spark.readstream and the autoloader.
