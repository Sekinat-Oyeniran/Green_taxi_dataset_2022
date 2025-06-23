
# Green Taxi Operations in NYC 
An analytical overview of trip volume, revenue patterns, and service behaviour in 2022

📌 Project Introduction

This project explores the operational dynamics of Green Taxis in New York City during 2022. Using real-world data from the NYC Taxi & Limousine Commission (TLC), the analysis uncovers patterns in rider behaviour, revenue generation, geographic demand, and time-based activity. The goal is to provide actionable insights to support urban planning, transportation policy, and business optimization.

🎯 Project Aim

• To analyze the trip patterns, peak periods, passenger demand, and revenue generation for NYC green taxis in 2022.

• To draw actionable insights from historical data using exploratory data analysis and data visualization techniques.

• To demonstrate end-to-end data engineering and analytics using an ETL and data wrangling approach.

🗂️ Data Source & Summary

Source: NYC Taxi & Limousine Commission (TLC) Open Data

Primary Dataset: Green Taxi Trip Records - 2022 (originally in Parquet format, processed using Python and read into CSV for ease of storage and chunked processing)

Supporting Dataset: Taxi Zone Lookup Table

The dataset includes: "Pickup & Drop-off Timestamps" "Location IDs" "Trip Distance & Passenger Count" "Payment Type, Fare Amount, and Total Amount" These records offer a detailed operational footprint of green taxi activity throughout NYC in 2022.

🧠 Project Overview

This project follows a structured data analytics pipeline that transforms raw NYC taxi data into actionable insights through the following stages:

• Ingest: Imported green taxi trip records and zone lookup tables into a database for processing and analysis.

• Extract & Transform: Cleaned data, handled nulls, standardized formats, and engineered new time-based features (month, hour, day).

• Load: Stored cleaned datasets in PostgreSQL, and later loaded into Power BI.

• Visualize: Built an interactive dashboard to reveal trip volume trends, revenue drivers, payment behaviour, and location-based demand.

[View the Dashboard Here](https://app.powerbi.com/groups/me/reports/d2ae0472-43f3-4898-9c42-a315b48dfe0a/2a6a68f982aa7711e3b2?bookmarkGuid=95cd190c-f38e-441d-88d0-439578983fc0&bookmarkUsage=1&ctid=bd697c1b-c481-479c-841e-c618542675c3&portalSessionId=bd1c34e3-9efb-4e63-b26e-436bbb6daae9&fromEntryPoint=export)

🧪 Methodology

Data Cleaning & Wrangling:

• Removed nulls and irrelevant rows

• Parsed and derived datetime components

• Mapped location IDs to boroughs/zones

• Standardized column types and values

ETL Pipeline Implementation:

• Python scripts were used to ingest, clean, and save transformed data.

• PostgreSQL was used for data storage and SQL queries for validation.

• Power BI was used for designing an interactive dashboard.

Data Modeling:

• Relationships created between trip data and zone lookup tables

• Measures and calculated columns added in Power BI for advanced analysis

🔍 Observations

• Trip volumes varied by day of the week, with Thursday recording the highest.

• Most trips were short in distance, with 1 to 2 passengers.

• Cash and credit card were dominant payment methods.

• Afternoon periods showed a spike in trip frequency and revenue generation.

📈 Key Insights from the Project

• Trip Volume by Day of the Week

Weekdays (Monday–Friday) showed consistently high taxi demand, peaking mid-week.

Sundays (Day 6) recorded the lowest number of trips (~95K), suggesting lower demand on weekends.

• Seasonal Trends in Taxi Trips

Trip volume peaked in spring (April–May), likely due to favorable weather.

A decline during summer (July–August) aligns with reduced city activity (e.g., vacations).

A recovery was observed in December, suggesting holiday-related travel.

• Most Active Boroughs by Taxi Zones

Manhattan and Queens had the highest number of active taxi zones, each with 69 unique pickup locations, reflecting centrality in transportation. Staten Island had the lowest (~20), indicating minimal green taxi activity.

• Payment Method Preferences by Trip Type

Trip Type 1 (likely street-hail or individual trips) had higher representation and used payment_type 1 (e.g., card) for 63% of payments.

Trip Type 2 (possibly dispatch or shared rides) leaned even more heavily on card payments (70.3%).

This suggests digital payments dominate green taxi transactions.

• Revenue Distribution by Time of Day

The afternoon period generated the highest revenue (~$5.26M) and also had the highest number of pickups, suggesting alignment between ride frequency and earnings during midday. Revenue dips during nighttime hours, which may suggest reduced activity or shorter trip distances.

✅ Strategic Takeaways & Recommendations

• High Weekday Demand (Peak on Thursdays)

Conclusion: Trips peak mid-week, especially on Thursdays.

Recommendation: Optimize fleet allocation and pricing strategies on high-demand weekdays.

• Afternoon Revenue Peak

Conclusion: Most revenue is generated in the afternoon.

Recommendation: Prioritize driver availability and manage traffic in busy zones during peak hours.

• Summer Dip in Ridership

Conclusion: Lower taxi usage in July–August suggests seasonal travel patterns.

Recommendation: Adjust fleet operations seasonally; launch off-peak promotions.

• Uneven Borough Demand

Conclusion: Manhattan and Queens see the most activity; Staten Island the least.

Recommendation: Improve service outreach and accessibility in underserved areas.

• Preference for Card Payments

Conclusion: Majority of trips are paid by card.

Recommendation: Strengthen digital payment systems; encourage cashless adoption.

• Trip Type Dominance

Conclusion: Trip Type 1 (street-hails) is heavily preferred.

Recommendation: Promote scheduled or app-based rides to enhance efficiency.





