# Udacity Data Modeling With Postgres

## Purpose:
This project was assigned using a subset of Sparkify song and log data to parse and load into a PostgreSQL database. I completed this as part of a Udacity nano degree in data analytics.

## File Structure
### The files in the repository are as follows:

#### sql_queries.py
This contains the queries that drops the tables if they exist, creates the tables, inserts extracted data from the datasets to the tables and a select query that gets the songid and artistid.

#### create_tables.py
This file contains the methods that execute the drop and create table queries found in the sql_queries file.

#### etl.py
Extracts data from the data files and inserts them in the database tables.

#### etl.ipynb
This is a testing file that uses 1 row at a time to ensure the sql_queries table was working, provided by Udacity

#### test.ipynb
This file provided by Udacity was used to connect to the database during the testing of etl.ipynb.

#### run_etl.ipynb
This file is for running the etl.py within JupyterLabs directly instead of in bash/cli

#### Data.zip
This file is a zip of the sub dataset provided to from Udacity with a log and user files with Json data

## Running Scripts
### Requirements
#### Python 3
Libraries Needed
os, glob, psycopg2, pandas as pd

##### Postgresql

Connect to your database, you may need to edit the scripts for your specific databate name.

To drop or create the tables, ensure you are in the project's directory then run the following command:

`python create_tables.py`
To run the ETL pipeline that will extract data from the datasets and store them in the tables simply run:

`python etl.py`
