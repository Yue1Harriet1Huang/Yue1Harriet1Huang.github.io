---
title: "Best Data Pipelines with Python Application"
author: yue
layout: post
permalink:
categories:
  - Data Engineering
  - Data Pipelines
excerpt: ""
---

## Database Comparison: 
- SQL-Server VS. Azure SQL DB
  - Migrate from On-Premise SQL-Server to Cloud Azure
- Google BigQuery VS. Azure Cosmos DB

## Python Pipeline: to On-Prem SQL-Server
- sqlcmd
- pyodbc 
- dask
- pyspark, koala

### pyodbc + pandas.read_sql()

### (pyspark's koala equivalent of read_sql)[https://stackoverflow.com/questions/38376307/create-spark-dataframe-from-sql-query]
> What is Databricks Koala
  - A high level wrapper of PySpark
  - What is its performance improvement from pandas sql? (size of data, speed, memory)
  - What is the gain you have only one machine/work from using koala over pandas
  - cannot be pyodbc + koala instead of jdbc
  - configure executor memory, configure master
  - What is a JDBC URI to use koalas.read_sql()
  - When use Koalas, you don't need to construct your own sparksession?
  
[Spark Dataframe Performance Benefits](https://www.data4v.com/spark-dataframe-performance-benefits/)

https://code.tubitv.com/introducing-tubi-data-runtime-387e8651d08a

#### Python Pipeline Comparison: sqlcmd VS. pyodbc

### [Data Serialization](https://martin-thoma.com/data-serialization/)

- yaml file
