Berikut versi **tanpa emoji**, rapi, dan profesional untuk README GitHub capstone project Module 2.

---

# Capstone Project – Module 2: Data Analysis

TransJakarta Payment Behavior & Usage Analytics

This repository contains the complete data analysis project for Capstone Module 2, focusing on understanding public transportation transaction patterns from TransJakarta. The project demonstrates the full workflow of data cleaning, exploratory data analysis (EDA), feature engineering, and dashboard development using Python and Tableau.

---

## 1. Project Overview

Public transportation systems produce large volumes of transactional data daily. Analyzing commuter behavior—such as payment trends, demographic patterns, trip frequency, and stop usage—provides valuable insights for improving service operations.

This project analyzes 37,900 TransJakarta transactions from April 2023 with a focus on:

* Payment behavior
* Age and demographic trends
* Bank usage
* Trip durations
* Geographic tap-in distribution
* Peak time activity
* High-frequency riders through Pareto analysis
* Corridor and stop-level insights

The final output includes a comprehensive Tableau dashboard designed for operational decision-making.

---

## 2. Data Cleaning and Preprocessing

Key steps performed:

* Converted invalid or inconsistent birth dates
* Fixed datatypes for datetime fields
* Removed outliers for trip duration
* Standardized stop names
* Engineered additional fields:

  * Hour of Day
  * Day of Week
  * Age
  * Age Groups (4-bucket segmentation)
  * Region classification (Jakarta Selatan, Utara, Barat, Timur, Pusat) using coordinates
* Prepared latitude and longitude fields for geospatial visualization in Tableau

---

## 3. Exploratory Data Analysis (EDA)

EDA was conducted using Python libraries (Pandas, NumPy, Matplotlib, Seaborn). Analyses included:

* Payment amount distribution
* Transaction count by bank
* User demographics (age, gender)
* Hourly and daily travel patterns
* Trip duration analysis
* Top tap-in stops
* Top corridors
* High-frequency rider analysis (80/20 distribution)
* Gender and age-specific payment patterns

---

## 4. Tableau Dashboard

A multi-dashboard Tableau visualization was built to highlight:

* KPI Scorecard (Total Trips, Revenue, Unique Riders, Average Payment, etc.)
* Payment Amount Distribution
* Payment by Age Group
* Hourly Usage Trend
* Geographic Tap-In Density Map
* Trip Duration by Time of Day
* Top Tap-In Stops by Transactions
* Frequent Users (Pareto Chart)
* Payment Behavior by Bank and Gender
* Dynamic filters and parameters for interactive analysis

Interactive controls include:

* PayCardBank
* Age Group
* Gender
* Corridor Name
* Date and Hour-Based Filters

---

## 5. Key Insights

Summary of insights generated:

* Approximately 80 percent of total transactions come from about 37 percent of users, indicating a strong concentration of high-frequency riders.
* Bank DKI is the dominant payment method across transactions.
* The majority of travelers fall within the 18–35 age range.
* Peak traffic occurs during 06:00–09:00 and 16:00–19:00.
* Geographic density analysis shows heavy tap-in activity in central business districts.
* A large volume of zero-payment transactions suggests special programs or incomplete tap sequences.

---

## 6. Tools and Technologies

* Python (Pandas, NumPy, Matplotlib, Seaborn)
* Jupyter Notebook
* Tableau Public
* Git and GitHub

---

## 7. Repository Structure

```
├── data/
│   ├── checked_transjakarta_dataset.csv
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   └── 03_feature_engineering.ipynb
│
├── tableau/
│   └── transjakarta_dashboard.twbx
│
├── README.md
```

---

## 8. Objectives

This project aims to demonstrate the ability to:

* Clean and preprocess real-world datasets
* Perform exploratory analysis and extract insights
* Conduct feature engineering
* Build geospatial and statistical visualizations
* Develop KPI-focused dashboards
* Communicate findings for business and operational improvements

