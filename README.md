# COVID-19 Data Analysis

Welcome to the COVID-19 Data Analysis repository! This project provides a series of SQL queries to analyze COVID-19 data, focusing on death rates, infection rates, and vaccination progress across various countries and continents.

## Overview

This repository contains SQL queries for analyzing COVID-19 data from the following perspectives:
- **Total Cases vs. Total Deaths**: Assessing the likelihood of death upon contracting COVID-19.
- **Total Cases vs. Population**: Determining the percentage of the population infected with COVID-19.
- **Highest Infection Rates**: Identifying countries with the highest infection rates relative to their population.
- **Highest Death Counts**: Analyzing countries with the highest total death counts.
- **Continental Analysis**: Examining death counts by continent.
- **Global Numbers**: Aggregating global COVID-19 cases and deaths.
- **Vaccination Analysis**: Tracking vaccination progress and its impact on population vaccination rates.

## Data Sources

The queries assume the existence of two primary tables:
- `dbo.CovidDeaths`: Contains data related to COVID-19 deaths.
- `dbo.CovidVaccinations`: Contains data related to COVID-19 vaccinations.

The structure of these tables is as follows:
- **CovidDeaths**: Location, Date, Total Cases, New Cases, Total Deaths, Population, Continent
- **CovidVaccinations**: Location, Date, New Vaccinations

## Queries

1. **Initial Data Inspection**
   - Review all columns with non-null continents and order data.
   - Retrieve selected columns for further analysis.

2. **Total Cases vs. Total Deaths**
   - Calculate the death percentage based on total cases for locations containing 'states'.

3. **Total Cases vs. Population**
   - Calculate the percentage of the population infected with COVID-19.

4. **Highest Infection Rate Compared to Population**
   - Identify countries with the highest infection rates relative to their population.

5. **Highest Death Count per Population**
   - Determine countries with the highest death counts.

6. **Death Counts by Continent**
   - Analyze continents with the highest death counts.

7. **Global Numbers**
   - Aggregate new cases and deaths globally and compute percentages.

8. **Join Tables and CTEs**
   - Merge COVID-19 deaths and vaccination data to analyze rolling vaccination numbers.

9. **Temporary Table and View Creation**
   - Create and use temporary tables and views for storing and querying vaccination progress.

## Usage

To use these queries:
1. Connect to your SQL database where the `dbo.CovidDeaths` and `dbo.CovidVaccinations` tables are located.
2. Execute the SQL queries as needed for your analysis.
3. Modify the queries if necessary to fit the schema of your database or to focus on specific regions or dates.

## Setup

1. **Database Setup**
   Ensure that you have access to a database with the required tables (`dbo.CovidDeaths` and `dbo.CovidVaccinations`).

2. **Query Execution**
   You can run the queries using any SQL client such as SQL Server Management Studio (SSMS), Azure Data Studio, or a similar tool.

## Conclusion

This repository provides SQL queries for comprehensive COVID-19 data analysis, enabling insights into infection rates, death counts, and vaccination progress across various regions.
