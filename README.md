# Automated-synchronization-of-staging-and-production-data-warehouse
Automated synchronization of staging data warehouse and production data warehouse. The Python script performs the incremental data load from MySQL server (staging data warehouse) to the PostgreSQL (production data warehouse). 

The script does the following tasks:
- Connect to PostgreSQL data warehouse and identify the last row on it.
- Connect to MySQL staging data warehouse and find all rows later than the last row on the datawarehouse.
- Insert the new data in the MySQL staging data warehouse into the PostgreSQL production data warehouse.

Files:
Original staging data warehouse: sales.sql
Original production data warehouse: sales.csv (in this case the table needs to be created, then load the data from the csv file)
Script for the automated sync up: automation.py
