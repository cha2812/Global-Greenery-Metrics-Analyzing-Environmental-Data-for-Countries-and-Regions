# Global-Greenery-Metrics-Analyzing-Environmental-Data-for-Countries-and-Regions
Analyzing environmental data related to land area and forest area across different countries and regions

## Introduction
The greenery dataset was provided with three(3) files which represented our tables. We have Regions, land area, and forest area which can be seen under the names **forest area.csv**, **land area.csv** and **regions.csv** in the file section and I performed data analysis using SQL. The dataset contains information about various countries, country codes, regions, forest square kilometres, total area square miles, year and income group details.

## Problem Statement
I wanted to find a way to understand the environment and things that affect it like deforestation, countries with large forests and the total area of countries. 
The following questions were asked and the answers were provided to questions and problems below.

1. Find the total number of countries involved in deforestation.
2. Show the income groups of countries having total area ranging from 75,000 to 150,000?
3. Retrieve the names of countries that have a forest area (in square kilometres) greater than the average forest area of all countries in the "High Income" income group.
4. Calculate the average total area (in square miles) for countries in the "Upper Middle Income" income group? Compare the result with the rest of the income categories.
Hint: calculate the average total areas for the 3 other categories.
5. Determine the total forest area (in square kilometres) for countries in the "High Income" income group? Also, compare with the other income categories.
6. What are the countries from each region or continent having the highest total forest area?


## Data Analysis
The analysis was done using three(3).csv files that were provided. The 3 tables provided were the Forest area table, the Land area table and the Regions table. <br>
The Forest area table had 4 columns; country code, country name, year and forest area per square kilometre. <br>
The Land area table had 4 columns; country code, country name, year and total area per square mile. <br>
The Regions table also had 4 columns; country name, country code, region and income group. <br>

The first step I took was to create a database called Greenery. After creating the Greenery Database, the next step was creating 3 tables named forest_area, land_area and regions. <br>
The Forest area table had 4 columns; country code, country name, year and forest area per square kilometre. <br>

![](pic1.png)

The Land area table had 4 columns; country code, country name, year and total area per square mile. <br>

![](pic2.png)

The Regions table also had 4 columns; country name, country code, region and income group. <br>

![](pic3.png)

The next step was to import the .csv files into the table to put rows and values into our table created. There are two ways to import files into the table in PostgreSQL.

Import the files by right-clicking on the table name on the right-hand side and then selecting Import/Export data and then selecting the location/folder where your .csv file is located and then importing. <br>
OR
Writing up a code or query in the query tool. The code to write is

COPY table_name

FROM 'file-path/location of file'

DELIMITER ','

CSV HEADER;




