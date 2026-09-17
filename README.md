# Employee Profile & Risk Analysis

## Project Overview

This project analyzes employee profiles and attrition patterns to identify factors associated with employee turnover.

The analysis uses employee demographic, employment, compensation, satisfaction, and tenure data. The project combines **Python/Pandas** for data preparation and preliminary exploration with **Power BI** for data modeling, analytical visualization, and interactive dashboard development.

The final output is an interactive Power BI dashboard designed to support HR-related monitoring and retention analysis.

---

## Business Problem

Employee attrition can affect workforce stability, operational continuity, and organizational costs.

This project aims to examine employee attrition patterns and identify groups or conditions associated with higher attrition. The analysis focuses on several employee characteristics, including:

- Age
- Department
- Job Role
- Monthly Income
- Years of Employment
- Overtime
- Job Satisfaction
- Environment Satisfaction
- Work-Life Balance
- Other employee profile characteristics

The analysis is intended to provide a data-driven overview that can support HR monitoring and retention planning.

---

## Objectives

The main objectives of this project are:

1. Measure the overall employee attrition rate.
2. Analyze attrition patterns across employee demographics and employment characteristics.
3. Examine attrition based on compensation, tenure, overtime, and satisfaction factors.
4. Identify employee groups with relatively higher attrition counts or rates.
5. Develop an interactive Power BI dashboard for HR monitoring and analysis.
6. Provide data-driven recommendations based on the observed patterns.

---

## Dataset

The dataset contains **1,470 employee records and 45 original variables** covering employee demographic, employment, compensation, and satisfaction information.

The dataset was obtained from **Kaggle** and prepared for analytical purposes.

Key variables include:

| Category | Examples |
|---|---|
| Demographics | Age, Gender, Marital Status, Education |
| Employment | Department, Job Role, Job Level, Years at Company |
| Compensation | Monthly Income, Stock Option Level |
| Work Conditions | Overtime, Business Travel, Distance from Home |
| Satisfaction | Job Satisfaction, Environment Satisfaction, Relationship Satisfaction, Work-Life Balance |
| Target | Attrition |

The repository also contains the processed Excel workbook used in the project, including the master data, fact table, and dimension tables.

---

## Data Preparation

Data preparation was performed using **Python/Pandas** and Power BI.

The main preparation steps included:

- Reviewing the structure and characteristics of the dataset.
- Removing constant or redundant columns such as:
  - `EmployeeCount`
  - `Over18`
  - `StandardHours`
- Creating employee identifiers.
- Creating grouped variables such as:
  - Age Group
  - Income Group
  - Distance Group
  - Years Group
- Preparing descriptive categories for satisfaction-related variables.
- Preparing categorical dimension tables for data modeling.

---

## Data Modeling

The project uses a **Star Schema** for the Power BI data model.

The model consists of:

- One fact table containing employee-level analytical records.
- Multiple dimension tables containing descriptive attributes.
- One-to-many relationships between dimension tables and the fact table.

The dimensional structure includes employee attributes such as:

- Attrition
- Business Travel
- Department
- Education
- Education Field
- Environment Satisfaction
- Gender
- Job Involvement
- Job Level
- Job Role
- Job Satisfaction
- Marital Status
- Overtime
- Performance Rating
- Relationship Satisfaction
- Stock Option Level
- Work-Life Balance

---

## Analysis Methodology

The analysis workflow consists of several stages:

### 1. Data Preparation

Python/Pandas was used to inspect and prepare the dataset before dashboard development.

### 2. Exploratory Analysis

Descriptive exploration was performed to understand employee characteristics and identify initial attrition patterns.

### 3. Data Modeling

The prepared data was structured into a Star Schema in Power BI.

### 4. KPI Development

Several DAX measures were created to monitor key HR indicators, including:

- Total Employees
- Total Attrition
- Attrition Rate
- Overtime Rate
- Overtime Employee
- Average Age
- Average Monthly Income
- Average Tenure
- Average Satisfaction

### 5. Diagnostic Analysis

Cross-tabulation and interactive filtering were used to examine attrition patterns across different employee characteristics.

---

## Dashboard

The Power BI dashboard provides an overview of employee profiles and attrition patterns.

### Dashboard 1 — Employee Profile & Risk Analysis

The dashboard covers:

- Total Employees
- Total Attrition
- Attrition Rate
- Average Age
- Average Monthly Income
- Average Years Worked
- Attrition by Department
- Attrition by Job Role
- Attrition by Education
- Attrition by Years Worked
- Attrition by Age
- Attrition by Monthly Income
- Attrition by Distance from Home
- Attrition by Overtime
- Attrition by Job Satisfaction
- Attrition by Environment Satisfaction
- Attrition by Work-Life Balance

---

## Key Findings

Based on the analysis:

- The dataset contains **1,470 employees**, with **237 employees recorded as having left**, resulting in an attrition rate of **16.12%**.
- Attrition was concentrated among employees with **less than five years of tenure**, with the highest count occurring during the first year.
- **R&D** recorded 133 attrition cases, while **Sales** recorded 92 cases.
- **Sales Executive** and **Research Scientist** were among the job roles with notable attrition counts.
- Employees working overtime had an attrition rate of **30.53%**, compared with **10.44%** among employees who did not work overtime.
- Employees with monthly income below **$3,000** recorded the highest attrition count.
- The **25–35 age group** recorded the highest attrition count, with 122 cases.
- Lower Job Satisfaction and Environment Satisfaction levels were associated with higher observed attrition counts.

> These findings describe observed patterns and associations in the dataset and should not be interpreted as proof of causal relationships.

---

## Recommendations

Based on the observed patterns, the analysis proposes several areas for HR consideration:

1. **Review compensation structures** for employees in lower-income groups.
2. **Evaluate workload and overtime allocation**, particularly in departments and roles with notable attrition.
3. **Strengthen onboarding and mentoring programs** for employees during their early tenure.
4. **Conduct regular employee engagement and satisfaction surveys** to monitor workplace conditions.
5. **Monitor attrition periodically** by department, job role, tenure, and other relevant employee characteristics.

---

## Tools & Technologies

- **Python**
- **Pandas**
- **Power BI**
- **DAX**
- **Microsoft Excel**

---

## Repository Structure

```text
employee-profile-risk-analysis/
│
├── README.md
│
├── dashboard/
│   ├── Hamida_Dashboard Employee Profile & Risk Analysis.pdf
│   └── Hamida_Dashboard Employee Profile & Risk Analysis.pbix
│
├── data/
│   └── HR-Employee-Attrition.xlsx
│
└── report/
    └── Hamida - Laporan Hasil Analisis Attrition Karyawan.docx.pdf
