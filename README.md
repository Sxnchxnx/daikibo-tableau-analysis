# daikibo-tableau-analysis
Data analysis of Daikibo telemetry data using Tableau dashboards and interactive visualizations.

# Daikibo Telemetry Data Analysis using Tableau

## Project Overview

This project analyzes telemetry data collected from four Daikibo factories during May 2021 using Tableau.

### Factories Analyzed
- Daikibo Factory Meiyo (Tokyo, Japan)
- Daikibo Factory Seiko (Osaka, Japan)
- Daikibo Berlin (Berlin, Germany)
- Daikibo Shenzhen (Shenzhen, China)

## Business Questions

1. Which factory experienced the most machine downtime?
2. Which machine types contributed most to downtime in that factory?

## Dataset

The dataset contains telemetry messages from 9 machine types across 4 factories.

Each machine sends a status update every 10 minutes.

### Source File
- daikibo-telemetry-data.json

## Tableau Analysis Steps

1. Imported JSON data into Tableau
2. Enabled all schema levels during import
3. Created calculated field:

```tableau
IF [Status] = "unhealthy" THEN 10 ELSE 0 END
```

Named as:

```
Unhealthy
```

4. Created:
   - Down Time per Factory bar chart
   - Down Time per Device Type bar chart

5. Built an interactive dashboard
6. Added factory filter action
7. Identified the factory with the highest downtime

## Dashboard

### Final Dashboard

![Dashboard](dashboard_screenshot.png)

## Key Findings

- Factory with highest downtime: [Replace with your result]
- Device type with highest downtime: [Replace with your result]

## Tools Used

- Tableau Desktop
- JSON Dataset
- Data Visualization
- Dashboard Design

## Repository Contents

| File | Description |
|--------|------------|
| dashboard_screenshot.png | Final dashboard screenshot |
| tableau_workbook.twbx | Tableau workbook |
| daikibo-telemetry-data.json | Dataset |
| Daikibo_Task_Guide.pdf | Project instructions |

## Author

Sinchana R

LinkedIn: https://www.linkedin.com/in/sinchana-r-788b1825b/
