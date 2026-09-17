# 📊 HR Analytics Dashboard — Employee Attrition Analysis

Analyzing employee attrition at a 1,800-person company using **Power BI** and **Excel**, built from
the same raw dataset — to compare and showcase both BI tools side by side.

![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=power-bi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

---

## 📌 Overview

This project analyzes why employees leave — using department, tenure, overtime, and job
satisfaction as the main risk factors — and presents the findings two ways:

- An **interactive Power BI dashboard** with DAX measures, slicers, and drill-down
- A **fully formula-driven Excel dashboard** (SUMIFS/COUNTIFS/AVERAGEIFS, no VBA) with its own
  interactive dropdown filters and charts

**Dataset:** 1,800 employees across 6 departments (Sales, R&D, HR, Finance, IT, Marketing), with
an overall attrition rate of ~18% — deliberately correlated with overtime, low job satisfaction,
short tenure, and frequent travel, so the analysis surfaces real, explainable patterns.

## 📂 Repository Contents

| File | Description |
|---|---|
| [`hr_employee_data.csv`](hr_employee_data.csv) | Raw dataset — 1,800 employees, 16 columns |
| [`HR_Analytics_Dashboard.xlsx`](HR_Analytics_Dashboard.xlsx) | Interactive Excel dashboard (Raw Data / Summary / Dashboard sheets) |


## 🔑 Key Questions Answered

1. Which departments have the highest attrition rate?
2. Does working overtime increase the chance of an employee leaving?
3. Is attrition concentrated in the first year, or spread evenly across tenure?
4. How strongly does job satisfaction predict attrition?
5. How has headcount grown year over year?

## 🔵 Power BI Dashboard

Built directly from `hr_employee_data.csv`. Includes:

- **KPI cards:** Total Employees, Attrition Rate, Avg Monthly Salary, Avg Tenure
- **Attrition Rate by Department** — bar chart, conditionally colored by risk level
- **Attrition Rate by Tenure Band** and **by Job Satisfaction Level**
- **Headcount by Gender** (donut) and **New Hires by Year** (line chart)
- **Department × Job Role matrix** for drill-down
- **Slicers:** Department, Gender, OverTime, Age Band


## 🟢 Excel Dashboard

`HR_Analytics_Dashboard.xlsx` has three sheets:

| Sheet | What's in it |
|---|---|
| **Raw Data** | Full dataset as an Excel Table, with formula-driven `Hire Year`, `Age Band`, and `Tenure Band` columns |
| **Summary** | SUMIFS / COUNTIFS / AVERAGEIFS breakdowns — attrition by department, tenure band, overtime status, and job satisfaction — with color-scale conditional formatting highlighting high-risk segments |
| **Dashboard** | Interactive dropdown filters (Department, Gender) driving live KPI cards and 3 charts that update automatically — no VBA, no macros, pure formulas |

Verified with a full recalculation: **5,508 formulas, zero errors.**

## 🧠 What This Project Demonstrates

- Translating a business question ("why are people leaving?") into a structured analysis
- Building the same insight two different ways (Power BI + Excel) — useful in any team, since
  not every stakeholder has Power BI access
- Writing defensive formulas / DAX measures that don't break when filtered to an empty subset
- Designing conditional formatting that highlights risk visually instead of just listing numbers


## 🧰 Tools Used

Power BI (DAX, calculated columns, slicers) · Excel (SUMIFS, COUNTIFS, AVERAGEIFS, conditional
formatting, interactive dashboards) 

---
