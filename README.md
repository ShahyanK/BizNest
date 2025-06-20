# BizNest
# BizNest – GTA Business Targeting Dashboard
BizNest is a Streamlit-based data exploration and business planning tool built to help aspiring entrepreneurs identify the most strategic GTA city to open a restaurant, using demographic data from Statistics Canada.

# Project Overview
This project visualizes and analyzes demographic data across 12 cities in the Greater Toronto Area (GTA) to assist users in choosing an optimal restaurant location based on key population metrics and business alignment scores.

# Data Source
The data was obtained from the official Statistics Canada Census 2021 profiles, such as:

https://www12.statcan.gc.ca/census-recensement/2021/dp-pd/prof/details/page.cfm?Lang=E&SearchText=mississauga&DGUIDlist=2021A00053521010,2021A00053520005,2021A000235,2021A00053521005&GENDERlist=1&STATISTIClist=1&HEADERlist=0

# Data Cleaning
The original census files included thousands of columns per city.

I created a custom processing script, BizNestDataProcessing, to:

Filter relevant demographic indicators (religion, age, household size, etc.)

Normalize values to percentages

Aggregate or bin similar values (e.g., age ranges)

Merge datasets across cities

# Final Output
A streamlined dataset with 44 essential indicators

Saved as: FinalData.csv

# Streamlit App
A Streamlit app (app.py) was developed to visualize and interact with the processed data.

Features:
City Demographics Tab:

Age group distribution

Religious affiliation

Median age and income

Restaurant Fit & Competition Tab:

Choose a restaurant category (e.g., Bubble Tea, Halal, Vegan)

See how well the city’s demographics match the typical customer profile

View a Business Targeting Fit Score out of 100

[Yelp API placeholder] for concentration of similar restaurants in the city

# Purpose
The goal of BizNest is to provide data-driven insights to help entrepreneurs, investors, and local business planners make smarter location decisions for launching new restaurants in the GTA.

By aligning restaurant types with the demographics of each city, users can reduce risk and increase the likelihood of finding the right customer base.

# Dataset
You can find all processed datasets in the datasets/ folder, including the main file:
datasets/FinalData.csv

# Tools & Libraries
Python (pandas, matplotlib)

Streamlit

Statistics Canada Census 2021 data

Excel

[Optional] Yelp Fusion API (planned)
