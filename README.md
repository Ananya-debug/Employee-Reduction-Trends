Project Overview

This project focuses on data cleaning, transformation, and exploratory data analysis (EDA) using SQL on a global layoffs dataset.
The goal was to standardize raw layoff records, remove inconsistencies, and extract meaningful workforce reduction insights across industries, countries, and companies.

Tech Stack

SQL (MySQL 8+)
Window Functions, CTEs, Aggregations
Data Cleaning & Transformation Queries

Steps Performed

1. Data Cleaning
Created staging tables to preserve raw data.
Removed duplicates using ROW_NUMBER() and CTEs.
Standardized company names, industries, and country fields.
Converted date strings into proper DATE datatype.
Handled NULL and blank values by propagating known values from similar companies.
Dropped unnecessary helper columns.

2. Exploratory Data Analysis (EDA)
Identified companies with the largest layoffs (single day & overall).
Analyzed layoffs by location, country, industry, and funding stage.
Calculated yearly and monthly layoff trends.
Built rolling totals of layoffs to track cumulative impact.
Ranked top companies per year using DENSE_RANK().

Key Insights

Startups with 100% layoffs often completely shut down.
Major industries impacted: Tech, Finance, Crypto, Retail.
Countries with the most layoffs: United States, India, United Kingdom.
Peak layoff years correspond to economic slowdowns & funding shortages.

How to Use
Clone the repository:
git clone 
Import the dataset into your MySQL instance.

Run the queries in sequence:
data_cleaning.sql → standardize & clean data.

eda_queries.sql → perform exploratory analysis.
