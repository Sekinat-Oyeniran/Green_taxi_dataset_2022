Green Taxi Operations in NYC - An analytical overview of trip volume, revenue patterns, and service behavior in 2022


📌 Project Introduction

This project explores the operational patterns of Green Taxis in New York City for the year 2022. The goal is to understand rider behavior, revenue trends, popular zones, and temporal dynamics across different boroughs using real-world NYC Taxi & Limousine Commission (TLC) trip data. The insights are intended to inform urban planning, transportation policy, and business decision-making.

🎯 Project Aim

* To analyze the trip patterns, peak periods, passenger demand, and revenue generation for NYC green taxis in 2022.

* To draw actionable insights from historical data using exploratory data analysis and data visualization techniques.

* To demonstrate end-to-end data engineering and analytics using an ETL and data wrangling approach.

🗂️ Data Source & Summary
  
Source: NYC Taxi & Limousine Commission (TLC) Open Data

Primary Dataset: Green Taxi Trip Records - 2022

Supporting Dataset: Taxi Zone Lookup Table

Format: Parquet

The dataset contains detailed trip-level information including:

"Pickup and drop-off timestamps", "Pickup and drop-off location IDs", "Trip distance", "Passenger count", "Payment and Fare Information"

This data provides a comprehensive view of green taxi operations in NYC throughout 2022. 

🧠 Project Overview

This project follows a structured data pipeline approach designed to prepare and analyze NYC Green Taxi trip data using modern data engineering and visualization practices. It transforms raw data into actionable insights through the following stages:

Ingest: The data was collected by importing raw NYC Green Taxi trip records and supporting lookup tables from the source into a database for storage, processing, and analysis.

Extract & Transform: Cleaned and prepared the data by handling nulls, converting data types, enriching it with new features (like month, day of week, and time of day), and joining zone lookup details.

Load: Saved the cleaned dataset into a relational database and later loaded it into Power BI for analysis.

Visualize: Built an interactive dashboard in Power BI to uncover patterns in trip volume, revenue trends, payment behaviors, and popular zones.

This streamlined process supports a better understanding of taxi operations and helps guide decision-making with real-world data.

🧪 Methodology

Data Cleaning & Wrangling:

* Removed nulls and irrelevant rows

* Parsed and derived datetime components

* Mapped location IDs to boroughs/zones

* Standardized column types and values

ETL Pipeline Implementation:

* Python scripts were used to ingest, clean, and save transformed data.

* PostgreSQL was used for data storage and SQL queries for validation.

* Power BI was used for designing an interactive dashboard.

Data Modeling:

* Relationships created between trip data and zone lookup tables

* Measures and calculated columns added in Power BI for advanced analysis









