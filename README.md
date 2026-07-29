This dashboard analyzing employee absenteeism : BMI impact, health reasons,monthly trends, and workload correlation
# HR Analytics: Absenteeism Dashboard 
<img width="1335" height="745" alt="image" src="https://github.com/user-attachments/assets/ee325725-cbb5-4dd7-8df2-ef03c8d6ea2d" />

## Overview
This Power BI dashboard analyzes employee absenteeism patterns and their correlation with health factors like BMI, smoking, and workload. Built using SQL for data preparation and Power BI for visualization to help HR reduce absenteeism and improve employee wellness.

## Features
1. **KPI Card**: 
   - Average Absenteeism Time: 6.92 hours
   
2. **BMI Impact Analysis**:
   - **Sum of Body_mass_index by BMI_Category**: Donut chart
     - Healthy weight: 9K (45.82%) - Highest
     - Obese: 7K (33.07%)
     - Overweight: 4K (21.11%)
   - **Insight**: Healthy weight employees have highest total BMI sum, followed by Obese

3. **Lifestyle Factors**:
   - **Count of Social_smoker**: Pie chart - 92.7% Non-smokers, 7.3% Smokers
   - **Sum of Pet by Pet**: Pie chart showing distribution of employees with pets

4. **Time-based Trends**:
   - **Absenteeism by Month**: Line chart showing peaks in Month 3 and Month 7
   - **Absenteeism by Day of Week**: Line chart - Highest on Day 2, decreases towards Day 5

5. **Workload Correlation**:
   - **Absenteeism vs Work_load_Average_day**: Scatter plot showing relationship between workload and hours absent

6. **Absenteeism Reasons**: Table slicer with health-related reasons
   - blood donation
   - Certain conditions originating in the perinatal period
   - Certain infectious and parasitic diseases
   - Congenital malformations
   - Diseases of the blood and immune system

## SQL Component
SQL scripts included for:
1. Data cleaning and transformation
2. Calculating BMI categories from height/weight
3. Aggregating absenteeism hours by month, day, reason
4. Joining employee health data with attendance records

## Dataset
Dataset includes HR absenteeism data with fields: Absenteeism_time_in_hours, Body_mass_index, BMI_Category, Social_smoker, Pet, Month_of_absence, Day_of_the_week, Work_load_Average_day, Reason

## Tools & Technologies
1. **SQL Server/MySQL** - Data extraction, cleaning, and transformation
2. **Power BI Desktop** - Dashboard design and DAX measures
3. **Power Query** - Data loading and shaping
4. **DAX** - KPI calculations: Average Absenteeism Time

## Key Insights
- **Average Absenteeism**: 6.92 hours per incident
- **BMI Factor**: Healthy weight employees contribute most to total BMI, but correlation with absenteeism needs deeper analysis
- **Smoking Impact**: Only 7.3% are social smokers
- **Peak Absence**: Months 3 and 7 show highest absenteeism hours
- **Weekly Pattern**: Mondays/Tuesdays have highest absenteeism
- **Health Reasons**: Infectious diseases and blood disorders are top reasons listed
