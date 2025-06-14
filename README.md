# Road Accident Dashboard

![Made with Excel](https://img.shields.io/badge/Made%20with-Excel-217346?logo=microsoft-excel&logoColor=white&style=flat)
![Data Cleaning](https://img.shields.io/badge/Data%20Cleaning-brightgreen?style=flat)
![Data Visualization](https://img.shields.io/badge/Data%20Visualization-orange?style=flat)
![Interactive Dashboard](https://img.shields.io/badge/Interactive%20Dashboard-blueviolet?style=flat)

---

## Overview

The **Road Accident Dashboard** is an Excel-based analytical tool offering detailed insights into road accident casualties for **2021 and 2022**. Raw data was carefully cleaned and prepared in Excel to ensure accuracy before being transformed into meaningful insights through interactive pivot tables and charts. This dashboard enables a wide range of stakeholders—including government transport agencies, emergency services, law enforcement, transport operators, traffic management authorities, and the public—to quickly assess key performance indicators related to accident severity, vehicle involvement, temporal trends, and environmental conditions. It supports data-driven decision-making to enhance road safety, improve emergency response planning, and guide policy development.

---

## Project Objectives

- Provide a high-level summary of total casualties as a core KPI.
- Analyze accident severity by category (Fatal, Serious, Slight) with percentage shares.
- Group casualties by vehicle type to identify high-risk vehicle categories.
- Compare monthly casualty trends between 2021 and 2022 to detect temporal changes.
- Identify road types with the highest casualty counts.
- Highlight top 5 districts with the highest casualties to pinpoint critical geographic areas.
- Assess casualty distribution across urban and rural areas to highlight location-based risks.
- Examine the impact of lighting conditions (Daylight vs Darkness) on casualties.
- Enable dynamic, interactive data exploration through timeline filters and slicers for enhanced user engagement. 

---

## Project Files

The following files are included in this project for demonstration and portfolio purposes:

- <a href="https://github.com/Arianne-R/road-accident-dashboard/blob/main/road_accident_raw_data.xlsb">**road_accident_raw_data.xlsb**</a> – Contains the original, unprocessed dataset of road accident casualties from 2021 and 2022, sourced from a publicly available database. This served as the basis for data cleaning and analysis.
- <a href="https://github.com/Arianne-R/road-accident-dashboard/blob/main/road_accident_dashboard.xlsb">**road_accident_dashboard.xlsb**</a> – Main project file where data was cleaned, structured, and analyzed using Excel features such as formatting, calculated columns, grouping, and PivotTables. Includes the completed interactive dashboard with visualizations, slicers, and timeline filters.
- <a href="https://github.com/Arianne-R/road-accident-dashboard/blob/main/dashboard_preview.png">**dashboard_preview.png**</a> – Preview image of the finalized Excel dashboard with visualizations and interactive elements.

---

## Data Preparation

### Data Cleaning & Transformation

- Corrected data inconsistencies and spelling errors (e.g., “Fetal” corrected to “Fatal”).  
- Standardized formats for casualty counts and accident dates.  
- Added calculated columns for **Month** and **Year** extracted from accident dates.  
- Removed duplicate records to ensure data integrity.  
- Created calculated fields in PivotTables for percentage shares (e.g., % by accident severity).  
- Grouped granular categories into broader segments using **Fields, Items, & Sets** in PivotTables:  
  - **Light Conditions**: Combined several “Darkness” types into one category:  
    - *Darkness – lighting unknown*  
    - *Darkness – lights lit*  
    - *Darkness – lights unlit*  
    - *Darkness – no lighting*  
    > Only “Daylight” and the grouped “Darkness” categories appear in the dashboard (individual items hidden).  
  - **Vehicle Types**: Consolidated vehicle types into grouped categories:  
    - **Cars**: "Car", "Taxi/Private hire car"  
    - **Bus**: "Bus or coach (17 or more seats)", "Minibus (8–16 seats)"  
    - **Van**: "Goods 7.5 tonnes mgw and over", "Goods over 3.5t and under 7.5t", "Van / Goods 3.5 tonnes mgw or under"  
    - **Motorcycle**: Four engine size categories (50cc–500cc+)  
    - **Others**: "Other vehicle", "Pedal cycle", "Ridden horse", "Agricultural vehicle"  
    > Original items hidden in PivotTables to display only grouped fields in visuals.  
- Converted cleaned dataset into Excel Table **AccidentData** for structured analysis.  

---

## Tools & Skills Demonstrated

| Skill / Tool          | Usage                                             |
|-----------------------|---------------------------------------------------|
| Excel PivotTables     | Aggregated accident and casualty data             |
| Slicers & Timeline    | Interactive filtering across multiple visuals     |
| Chart Types           | Donut, line, clustered bar, and column charts     |
| Excel Tables          | Structured dataset for reliable Pivot analysis    |
| Data Storytelling     | Insights supported by visuals and KPIs            |
| Grouping Techniques   | Consolidated vehicle types and lighting conditions|  

---

## Key Dashboard Features

**1. Total Casualties**  
Summarizes total casualties as a key KPI using a pivot table.

**2. Casualties by Accident Severity**  
Breaks down casualties by severity categories (Fatal, Serious, Slight) with percentages, visualized via donut charts.

**3. Casualties by Vehicle Type**  
Groups related vehicle types into consolidated categories (Cars, Bus, Van, Motorcycle, Others) sorted by casualty count.

**4. Monthly Trend Comparison (2021 vs 2022)**  
Displays monthly casualty trends over two years with a line chart.

**5. Casualties by Road Type**  
Identifies road types with the highest casualties, visualized through clustered bar charts.

**6. Top 5 Districts by Casualties**  
Highlights districts with the most casualties via clustered column charts.

**7. Casualties by Area Type**  
Compares casualties across urban and rural areas to reveal location-based risks.

**8. Casualties by Light Conditions**  
Consolidates lighting conditions into Daylight vs Darkness categories, visualized with donut charts.

**9. Interactive Features**

- **Timeline control** connected to multiple PivotTables for dynamic filtering by date, including:  
  - Total Casualties  
  - Casualties by Accident Severity  
  - Casualties by Vehicle Type
  - Monthly Trend (2021 vs 2022)  

- **Urban/Rural Area slicer** connected to PivotTables for filtering by area type across:  
  - Total Casualties  
  - Casualties by Accident Severity  
  - Casualties by Vehicle Type  
  - Monthly Trend (2021 vs 2022)  
  - Maximum Casualties by Road Type  
  - Top 5 Districts with Highest Casualties  
  - Casualties by Area Type  
  - Casualties by Light Conditions  

> The Urban/Rural Area slicer filters the Top 5 Districts with Highest Casualties because each district contains data broken down by area type. This allows the district rankings to dynamically reflect casualties by the selected area classification.

These interactive controls allow users to explore and analyze the data dynamically by filtering multiple visuals simultaneously.

---

## Dashboard Preview

![dashboard_preview](https://github.com/user-attachments/assets/1010fd99-4a3d-41f9-bda1-e9cdcb4e37f1)


> Dynamic Excel dashboard with timeline and slicers, designed to explore casualty trends and identify high-risk factors in road accidents.

---

## Dashboard Insights

> **Note:** The insights below are based on the full, unfiltered dataset and do not change when using slicers or the timeline.  
> While the dashboard supports interactive filtering by date and area type, these insights reflect the overall picture prior to applying any filters.

### Casualties by Vehicle Type

Cars accounted for nearly **80%** of casualties.  
Other vehicle types such as motorcycles, vans, and buses had substantially fewer casualties, highlighting the dominance of cars in road incidents.

### Monthly Casualty Trend Comparison (2021 vs 2022)

Casualties in **2022** were generally lower than in **2021** across months, indicating improved road safety.  
The largest month-over-month difference was in **December**, with over **5,300 fewer casualties** in 2022.

### Casualties by Road Type

The majority of casualties occurred on **Single carriageways**, accounting for approximately **74%** of total incidents.  
This highlights the increased risk associated with this road type compared to dual carriageways or roundabouts.

### Top 5 Districts with Highest Casualties

- **Birmingham** recorded the highest casualty count, with over **8,600 incidents**.  
- Other top districts include **Leeds, Bradford, Manchester,** and **Liverpool**, indicating major urban centers as high-risk areas.

### Casualties by Area Type

Casualties were significantly higher in **Urban areas** (approximately **61%**) than Rural, likely due to greater traffic volume and population density in cities.

### Casualties by Light Conditions

The majority of casualties occurred in **Daylight**, totaling over **304,000** incidents, which accounts for approximately **73%** of all casualties.
Casualties in **Darkness** (about **27%**) were notably fewer, suggesting that while night driving carries risk, most incidents happen during daytime when road activity is higher.

---

## How to Use

1. **Open** `road_accident_dashboard.xlsb` in Microsoft Excel (desktop version recommended for full functionality). 
2. **Navigate to** the `Dashboard` worksheet to view and interact with visualizations.
3. **Use** slicers and the timeline to filter data by date range and area type.  
4. **Explore** pivot charts and KPI summaries across the dashboard.  
5. **Hover** over visual elements to access additional insights where available.  
6. **Refer** to `road_accident_raw_data.xlsb` to audit or reanalyze the original dataset.

---

## Explore the Dashboard

The Road Accident Dashboard demonstrates how Excel can be used to turn raw traffic incident data into a meaningful tool for monitoring road safety. From identifying high-risk vehicle types and accident hotspots to visualizing the impact of environmental factors like lighting and area type, this project highlights how interactive dashboards can support safer roads and smarter policy decisions. It reflects my hands-on experience with data cleaning, transformation, and visualization in a real-world context.

For questions or further discussion, please don’t hesitate to connect with me via LinkedIn (link available in my GitHub profile).

---
