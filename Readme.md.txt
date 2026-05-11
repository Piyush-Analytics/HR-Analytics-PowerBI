# 👥 HR Analytics Dashboard (Power BI)

![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📌 Overview
Interactive Power BI dashboard analysing IBM HR Employee Attrition dataset 
(1,470 employees, 35 features) — covering attrition drivers, department 
analysis, gender diversity, overtime impact and tenure patterns.

## 📊 Dashboard Preview
![HR Analytics Dashboard](HR_Analytics_PowerBI_Dashboard.png)

## 📈 Key Metrics
- Total Employees: **1,470**
- Attrition Count: **237**
- Attrition Rate: **16.1%**
- Avg Monthly Income: **$6,503**
- Avg Tenure: **7.01 years**

## 🔍 Key Insights
- Overtime workers leave at **30.5% vs 10.4%** — 3x higher risk
- **Sales department** has highest attrition (92 employees)
- **Laboratory Technicians** are the most at-risk job role (62 left)
- **60% Male vs 40% Female** workforce split
- Employees with **0-2 years tenure** leave most frequently

## 📊 Dashboard Features
- 5 KPI Cards — Total Employees, Attrition Count, Attrition Rate %, Avg Income, Avg Tenure
- 6 Interactive Charts — Bar, Column, Donut, Horizontal Bar
- 3 Slicers — Department, Gender, Job Role
- Cross-filtering — clicking any chart filters all visuals

## 🛠️ DAX Measures
| Measure | Formula |
|---------|---------|
| Total Employees | `COUNTROWS(table)` |
| Attrition Count | `CALCULATE(COUNTROWS, Attrition = "Yes")` |
| Attrition Rate % | `DIVIDE([Attrition Count], [Total Employees])` |
| Avg Monthly Income | `AVERAGE(MonthlyIncome)` |
| Avg Tenure | `AVERAGE(YearsAtCompany)` |

## 🛠️ Tools Used
- Power BI Desktop
- DAX
- Power Query

## 📂 Dataset
[IBM HR Analytics — Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)