# Project 1: Data modeling with Postgres

### Introduction
A startup called **Sparkify** wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis, and bring you on the project. Your role is to create a database schema and ETL pipeline for this analysis. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.

### Project Description
In this project, you'll apply what you've learned on data modeling with Postgres and build an ETL pipeline using Python. To complete the project, you will need to define fact and dimension tables for a star schema for a particular analytic focus, and write an ETL pipeline that transfers data from files in two local directories into these tables in Postgres using Python and SQL.

## project Database: 
- Song Dataset
- Log Dataset

### Schema_design 
 star schema has 1 fact table (songplays), and 4 dimension tables (users, songs, artists, time). 
Blankdiagram.png
![Schema_design](Images/example.png)
https://r766469c826263xjupyterllyjhwqkl.udacity-student-workspaces.com/files/Blankdiagram.png?_xsrf=2%7Cd6dc5ca7%7C2db87b53d8cc0b37e62487f27aca0064%7C1624476161


- must run create_tables.py before start to create your database and tables. then sql_queries.py to CREATE/Drop statements in for each table.

## Library:
- import os
- import glob
- import psycopg2
- import pandas as pd

## Song play example queries:
- SELECT first_name ,  FROM Song


## to run the program 
- run python create_tables.py  python etl.py