# Data Jobs Dashboard

Interactive Power BI dashboard analyzing global trends in the data jobs market using data visualization and business intelligence techniques.

---

## Project Overview

This dashboard was built to analyze:
- Job demand trends
- Salary distribution
- Geographic hiring patterns
- Job platform insights
- Work structure and employment types

The project focuses on transforming raw datasets into meaningful and actionable insights through interactive visualizations.

---

## Tools & Technologies

- Power BI
- Power Query
- DAX
- Data Cleaning
- Data Visualization

---

## Dashboard Features

- KPI Cards
- Interactive Filters
- Drill-through Analysis
- Geographic Job Mapping
- Salary Trend Analysis
- Platform Comparison
- Job Category Insights

## Data Source
 
The report is built on a single flat table: **`job_postings_flat`**
 
Key columns used across visuals:
 
| Column | Description |
|--------|-------------|
| `job_title_short` | Standardised job title (e.g. Data Analyst, Data Engineer) |
| `salary_year_avg` | Average yearly salary |
| `salary_hour_avg` | Average hourly salary |
| `job_posted_date` | Posting date (used for year/quarter hierarchy) |
| `job_country` | Country of the posting |
| `job_via` | Platform the job was posted on |
| `job_schedule_type` | Full-time / part-time / contract |
| `job_work_from_home` | Boolean — remote-eligible |
| `job_health_insurance` | Boolean — health insurance offered |
| `job_no_degree_mention` | Boolean — degree not mentioned as requirement |
 
---
## Dashboard Preview

### Main Dashboard
![Dashboard Overview](Images/dashboard-overview.png)

### Global Analysis
![Global Analysis](Images/global-analysis.png)

### Drill Through Analysis
![Drill Through](Images/drillthrough-analysis.png)

---

## Learning Source

Concepts and workflow inspired by Luke Barousse’s Data Analyst Course.

---

## Files Included

| File | Description |
|---|---|
| `Project_1.pbix` | Main Power BI dashboard |
| `dataset.csv` | Dataset used for analysis |
| `Images/` | Dashboard screenshots |

---
 
## How to Use
 
1. Open `Project_1.pbix` in **Power BI Desktop** (May 2026 or later recommended).
2. Use the **Job Title** dropdown slicer to filter all visuals to a specific role.
3. From the overview table or bar chart, click a job title and then **Drill through to Job Title** to land on Page 2 pre-filtered.
4. Hover over any visual for tooltips with exact figures.
5. Use the map on Page 2 to explore global posting concentration.
---
 
## Requirements
 
- Power BI Desktop (free) — [download here](https://powerbi.microsoft.com/desktop)
- For the Esri map visual: an ArcGIS Maps for Power BI account (free tier available)
- No external data connection required — data is embedded in the `.pbix` file
---

## Key Learnings

- Building interactive dashboards
- Creating analytical layouts
- Using DAX for calculated insights
- Implementing drill-through navigation
- Improving visual storytelling

---

## Author

Utkarsh Yadav
