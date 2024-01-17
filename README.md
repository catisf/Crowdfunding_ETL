# Crowdfunding_ETL
# Project 2 Group 1 - Extract, Transform and Load

## Overview
This project is part of the UoB Analyses Bootcamp. The main aim of the project was to collaboratively perform Extract, Transform and Load (ETL) operations. As part of the project, we extracted data from provided excel files, cleaned, transformed (including splitting columns, creating and merging pandas dataframes, changing date types, etc.), and saved it. We then created a SQL database with the cleaned datasets. These analyses involved using Python, Pandas, Numpy and PG admin.

<p align="center">
  <img src = "https://github.com/catisf/Crowdfunding_ETL/blob/main/sql_database/crowdfunding_erd.png" height = "75%" width = "75%">
</p>
                                                    Fig1 - Entity Relationship Diagram (ERD) for the Crowdfunding database

## Repository structure:
This repository contains:
- Jupyter notebook [ETL_Mini_Project_CFerreira_GAnyasor_EKobyaImanci.ipynb](https://github.com/catisf/Crowdfunding_ETL/blob/main/ETL_Mini_Project_CFerreira_GAnyasor_EKobyaImanci.ipynb), which contains the code to clean, transform and save the data
- Folder [sql_database](https://github.com/catisf/Crowdfunding_ETL/tree/main/sql_database) containing:
  - [png file](https://github.com/catisf/Crowdfunding_ETL/blob/main/sql_database/crowdfunding_erd.png) with the database's Entity Relationship Diagram (ERD)
  - [a sql file](https://github.com/catisf/Crowdfunding_ETL/blob/main/sql_database/crowdfunding_db_schema.sql) reflecting the database's schema
  - [the code](https://github.com/catisf/Crowdfunding_ETL/blob/main/sql_database/display_data.sql) used to display the data on PG admin, once it had been imported to each table
  - [folder PGAdmin_screenshots](https://github.com/catisf/Crowdfunding_ETL/tree/main/sql_database/PGAdmin_screenshots) with screenshots of PGAdmin data.
- Folder [Resources](https://github.com/catisf/Crowdfunding_ETL/tree/main/Resources) containing:
    - 2 '.xlsx' files, with the original data provided
    - 4 '.csv' files, with the cleaned and transformed data.

## Set up and execution
1. Clone the repository to your local computer: in your Terminal type `git clone https://github.com/catisf/Crowdfunding_ETL.git` 

2. Jupyter notebook:
- To run the jupyter notebook you will need to install the following packages:
   - jupyter notebook `pip install notebook`
   - pandas `pip install pandas`
   - numpy `pip install numpy`
   - json `pip install jsons`

3. SQL database:
- In order to create the database:
  - install PGAdmin
  - add a new database (e.g. named 'crowdfunding_db')
  - use the [sql_file in the sql_database folder](https://github.com/catisf/Crowdfunding_ETL/blob/main/sql_database/crowdfunding_db_schema.sql) to create the necessary tables
  - import the data using the csv files in the [resources folder](https://github.com/catisf/Crowdfunding_ETL/tree/main/Resources)

> [!TIP]
> Make sure you import the data in the same order that the tables were created. 
    
  - check the data has been imported correctly by running [the code](https://github.com/catisf/Crowdfunding_ETL/blob/main/sql_database/display_data.sql) in the sql_database folder.
 
## Data Source
- https://github.com/catisf/Crowdfunding_ETL.git
- Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.

## Authors
The following authors worked collaboratively on this project:
- [Catarina Ferreira](https://github.com/catisf)
- [Elcin Kobya Imanci](https://github.com/ELCINKOBYAIMANCI)
- [Godswill Anyasor](https://github.com/AnyasorG)
