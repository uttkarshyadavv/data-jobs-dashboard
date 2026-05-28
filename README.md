# Data Jobs Dashboard — Power BI

> Interactive exploration of global data job market trends — salaries, demand, benefits, platforms, and geography.

---

## Project Overview

This dashboard was built to analyze the data jobs landscape through interactive, filterable visuals across two report pages. It transforms raw job posting data into actionable insights across:

- Job demand trends by title and time
- Salary distribution (yearly and hourly)
- Geographic hiring patterns
- Job platform and sourcing insights
- Work structure and employment types
- Benefits availability (health insurance, remote work, degree requirements)

Inspired by Luke Barousse's Data Analyst Course.

---

## Dashboard Pages

### Page 1 — Overview

High-level summary focused on job volume and compensation trends.

| Visual | Type | Description |
|--------|------|-------------|
| Job Count & Avg Salary | KPI Cards | At-a-glance summary metrics |
| Salary Aggregates | KPI Cards | Total yearly and hourly salary figures |
| Postings Over Time | Line Chart | Job volume by year and quarter |
| Salary by Role | Scatter Plot | Hourly vs. yearly salary — reveals compensation clusters |
| Job Count by Title | Clustered Bar | Ranked job volume across all roles |
| Summary Table | Table | Job title, total postings, and total salary |
| Job Title Slicer | Dropdown Filter | Isolates any single role; synced with Page 2 |
| Drill-through Button | Navigation | Jump to Page 2 filtered to selected title |

---

### Page 2 — Job Details

Deeper dive into benefits, platforms, work arrangements, and global distribution.

| Visual | Type | Description |
|--------|------|-------------|
| Yearly Salary Gauge | Gauge | Actual vs. median yearly salary |
| Hourly Salary Gauge | Gauge | Actual vs. target hourly salary range |
| Degree Requirement | Donut Chart | Share of postings with no degree mentioned |
| Health Insurance | Donut Chart | Share of postings offering health insurance |
| Remote Work | Donut Chart | Work-from-home vs. on-site split |
| Postings by Platform | Clustered Bar | Volume by `job_via` source |
| Schedule Type | Treemap | Full-time / part-time / contract distribution |
| Country Heatmap | Esri ArcGIS Map | Geographic density of job postings |
| Job Title Slicer | Dropdown Filter | Synced with Page 1 |

---

## Features

- **Cross-page slicer sync** — Job Title filter on both pages is linked; selecting a role on Page 1 carries over to Page 2.
- **Drill-through navigation** — Click any title in the bar chart or table, then use the drill-through button to land on the detail page pre-filtered.
- **Interactive tooltips** — Hover over any visual for exact figures.
- **Esri ArcGIS map** — Global posting heatmap by country (requires ArcGIS account).

---

## Data Source

Single flat table: **`job_postings_flat`**

| Column | Description |
|--------|-------------|
| `job_title_short` | Standardised job title (e.g. Data Analyst, Data Engineer) |
| `salary_year_avg` | Average yearly salary |
| `salary_hour_avg` | Average hourly salary |
| `job_posted_date` | Posting date — used for year/quarter hierarchy |
| `job_country` | Country of the posting |
| `job_via` | Platform the job was posted on |
| `job_schedule_type` | Full-time / part-time / contract |
| `job_work_from_home` | Boolean — remote-eligible |
| `job_health_insurance` | Boolean — health insurance offered |
| `job_no_degree_mention` | Boolean — no degree mentioned as a requirement |

---

## Tools & Technologies

- **Power BI Desktop** — report creation and publishing
- **Power Query** — data ingestion and transformation
- **DAX** — calculated measures and KPIs
- **Esri ArcGIS Maps** — geographic visualisation

---

## Dashboard Preview

### Main Dashboard
![Dashboard Overview](Images/dashboard-overview.png)

### Global Analysis
![Global Analysis](Images/global-analysis.png)

### Drill-through Analysis
![Drill Through](Images/drillthrough-analysis.png)

---

## How to Use

1. Open `Project_1.pbix` in **Power BI Desktop** (May 2026 or later).
2. Use the **Job Title** dropdown slicer to filter all visuals to a specific role — the filter syncs across both pages.
3. From the bar chart or summary table on Page 1, select a title and click **Drill through to Job Title** to land on Page 2 pre-filtered to that role.
4. Hover over any visual for tooltips with exact figures.
5. On Page 2, use the Esri map to explore global posting concentration by country.

---

## Requirements

- [Power BI Desktop](https://powerbi.microsoft.com/desktop) (free)
- ArcGIS Maps for Power BI account for the map visual (free tier available)
- No external data connection required — data is embedded in the `.pbix` file

---

## Files

| File | Description |
|------|-------------|
| `Project_1.pbix` | Main Power BI dashboard |
| `dataset.csv` | Source dataset |
| `Images/` | Dashboard screenshots |

---

## Key Learnings

- Building interactive, multi-page Power BI dashboards
- Cross-page slicer sync and drill-through navigation
- DAX for calculated KPIs and measures
- Geographic visualisation with Esri ArcGIS
- Visual storytelling with data — layout and hierarchy

---

## Author

**Utkarsh Yadav**  
Chemical Engineering · ML/AI · SVNIT Surat  
[LinkedIn](https://linkedin.com/in/utkarsh-yadavv) · [GitHub](https://github.com/uttkarshyadavv)
