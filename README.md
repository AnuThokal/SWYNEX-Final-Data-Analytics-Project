# Final Data Analytics Project 

## Project Overview 

-This project is a **Final Data Analytics Project** built using **Power BI**, with **Excel** and **Power Query** for data preparation.
-The dataset has **465 patient records** across **Neurology, Orthopedics, General and Cardiology** departments.
-It covers the full process, from cleaning raw data to building visuals and drawing business insights.
-It helped strengthen practical skills in **Power BI, data cleaning and data-driven decision making**.

# Problem Statement:

Hospitals handle large amounts of patient and billing data every month, but without a proper reporting system, tracking performance is hard.
Management often cannot easily see total revenue, patient load, or how each department and doctor is performing.
Trends across months and quarters are hard to spot from raw data alone.
This project builds an interactive Power BI dashboard that brings all this data into one view.
It shows total revenue, patient count, monthly trends, and department and doctor performance.
It also breaks down patients by gender and age group.
This makes the data easy to read and use for quick, informed decisions.

# Dataset Information :

The messy_clinic_appointments dataset contains 465 hospital patient and billing records across four departments — Neurology, Orthopedics, General and Cardiology — covering 12 months (January to December).

download link: 
[messy_clinic_appointments.csv](https://raw.githubusercontent.com/AnuThokal/SWYNEX-Final-Data-Analytics-Project/refs/heads/main/messy_clinic_appointments.csv)

# Data Cleaning Process :
Before building the dashboard, the raw data was checked and cleaned in Excel and Power Query:
- Removed null and error values found in the dataset
- Replaced missing values in the gender column with "Not Specified"
- Standardized inconsistent text casing (male/Male, female/Female)
- Applied a custom Power Query formula to correct the date column, which had a mix of text, datetime, and multiple regional formats
- Detected and converted mixed-currency billing amounts (€, £, $) into a single currency
-  Created an Age Group column from age (0-18, 19-35, 36-60, 60+) and built a Pivot Table showing department-wise patient counts by gender
- Verified no rows were lost in the process — final dataset: 465 rows, 11 columns.

  Before cleaning process:
  <img width="1920" height="1000" alt="Screenshot (68)" src="https://github.com/user-attachments/assets/fbe916f1-3d84-4efb-9c32-ee7d9750c93d" />

  After cleaning process:
  <img width="1920" height="1080" alt="Screenshot (66)" src="https://github.com/user-attachments/assets/d2d42623-73fe-46c6-b7be-ca33eb1bf985" />

# Analysis:
Once the data was clean, the following analysis was carried out:
-Monthly revenue trend — to see which months performed best and worst
-Department-wise revenue and patient distribution — to compare four departments side by side
-Top 5 doctors by revenue — to identify the strongest revenue contributors
-Gender distribution across age groups — Adult, Senior and Teenager
-Quarter-wise comparison — using Qtr 1 to Qtr 4 filters for deeper exploration.













