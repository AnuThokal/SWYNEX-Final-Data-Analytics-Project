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

##  Data Analysis :
Once the data was clean, the following analysis was carried out:

**Monthly Revenue Trend**
<img width="320" height="147" alt="92" src="https://github.com/user-attachments/assets/53f10b69-70e2-424f-b4b9-bbb9c047b22f" />

Revenue moved up and down through the year instead of following one steady direction. It rose from January to February (537K to 789K), then dropped sharply in March and stayed lower through April. From May to August, revenue increased steadily each month, reaching 610K, before falling sharply again in September to the year's lowest point (301K). It picked up again from October to November before dipping slightly in December.

**Department-wise Revenue and Patients**
.<img width="156" height="146" alt="93" src="https://github.com/user-attachments/assets/21a340da-917b-4d5d-a44d-b3b7209a4033" />

Revenue is not equal across departments even though patient numbers are close. Neurology brings in the highest revenue (1794K) and Cardiology the lowest (1066K), a difference of over 700K. But patient counts stay almost the same across all four departments (109 to 119), so the gap comes from higher earnings per patient in Neurology, not more patients

**Top 5 Doctors by Revenue**
<img width="272" height="104" alt="doctor chart" src="https://github.com/user-attachments/assets/2b1dfbd1-ca66-4918-b9c8-863cba64c5fe" />

The top 5 doctors are very close in performance, with only a 1K difference between the highest (Emily Barnes, 48K) and the lowest (Kathryn Young, 47K). This shows revenue is spread evenly among top doctors rather than one person driving most of it.

**Gender Distribution Across Age Groups**
<img width="320" height="125" alt="77" src="https://github.com/user-attachments/assets/565caea3-8e44-4846-abba-884580e56e2a" />

Female patients are higher than male patients in the Adult group (134 vs 106), a positive gap of 28. In the Senior group, the numbers are almost equal (107 female vs 105 male). In the Teenager group, male patients are slightly higher (8 vs 5), though this group is very small overall.

**Quarter-wise Comparison**
<img width="239" height="153" alt="94" src="https://github.com/user-attachments/assets/232ddbf9-15c5-44ea-908b-2b531902e0fd" />

Revenue was highest in Quarter 1 (1747K) and dropped in Quarter 2 (1327K), a decrease of about 420K. It rose again in Quarter 3 (1442K) and continued rising into Quarter 4 (1498K), but stayed below the Quarter 1 level for the rest of the year.

##  Dashboard :
**1.Data Exploratory analysis dashboard:**
<img width="1920" height="1080" alt="Screenshot (77)" src="https://github.com/user-attachments/assets/d11c91a4-62cb-4e96-8a34-7e644c0e0e78" />

-Month & Department Slicers – Filter the whole dashboard by month or department; every chart updates instantly.
-Patients: Male vs Female – Compares male and female patient counts across Adult, Senior, and Teenager groups.
-Department Wise Total Amount (Waterfall) – Shows each department's share of total billing, building up to the grand total of ₹60,16,286.
-Amount by Quarter – Breaks down billing by quarter, with Qtr1 as the highest at ₹17,48,197.
-Department Wise Patient (Treemap) – Shows patient distribution by department — Neurology and Orthopedics lead with 119 each.

**2.Patient and Revenue dashboard:**
This Power BI dashboard gives a complete view of hospital revenue and patient data on a single page.
<img width="1276" height="726" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/68cba2ef-7ba5-4021-bad1-b638f3a44756" 

- Sum of Amount (KPI Card) — Shows total revenue earned, ₹6.01629M.
- Total Patients (KPI Card) — Shows total patients treated, 465.
- Quarter Filter (Qtr 1–Qtr 4) — Buttons to filter the whole dashboard by quarter.
- Amount by Month (Column Chart) — Revenue for each month; highest in February (789K), lowest in September (301K).
- Top 5 Doctors by Amount (Bar Chart) — Top 5 revenue-generating doctors, ranging from 47K to 48K.
- Amount by Department (Donut Chart) — Revenue share by department; Neurology highest (1794K), Cardiology lowest (1066K).
- Department wise Patients (Treemap) — Patient count per department, ranging from 109 to 119.
- Patients: Male vs Female (Clustered Column Chart) — Gender split across Adult, Senior and Teenager age groups.

  ## Key Business Insights :
-February had the highest revenue (789K) and September the lowest (301K)
-Neurology earns the most (1794K), while Cardiology earns the least (1066K)
-Patient counts are almost equal across departments (109 to 119), so Neurology earns more per patient rather than from higher patient volume
-The top 5 doctors are close in performance, all between 47K and 48K
-Adults (240) and Seniors (212) make up almost all patients; Teenagers are only 13
-Female patients (246) are slightly more than male patients (219)

## Tools Used:

| Tool | Purpose |
|------|---------|
| Excel | Initial data checking and cleaning |
| Power Query | Data transformation and cleaning |
| Power BI Desktop | Building the dashboard and visuals |














