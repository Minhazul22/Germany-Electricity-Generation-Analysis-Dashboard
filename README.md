# Germany Electricity Generation Analysis Dashboard

An interactive Power BI dashboard for exploring Germany's electricity generation patterns, renewable energy trends, and electricity mix using hourly market data from **SMARD (Bundesnetzagentur)**.

## Project Overview

This project analyses electricity generation in Germany across renewable and conventional energy sources. It brings time-series data into an interactive Power BI report so users can explore how generation changes over time, compare energy sources, and understand the contribution of renewables to the overall electricity mix.

**Tools and technologies:** Power BI · Power Query · DAX · Microsoft Excel · SMARD Open Data

## Dashboard Preview

The screenshot supplied for this project can be added at `assets/dashboard-preview.png`. Once you add that image to the repository, you can embed it here:

```markdown
![Germany Electricity Generation Dashboard](assets/dashboard-preview.png)
```

## Dashboard Highlights

- **Headline KPIs:** Total electricity generation, total wind generation, onshore wind, offshore wind, and photovoltaic generation.
- **Generation trends over time:** Hourly generation by energy source, with date-range and category filtering.
- **Electricity generation mix:** A breakdown of the contribution made by the selected energy sources.
- **Monthly wind comparison:** Onshore and offshore wind generation compared across the calendar year.
- **Monthly energy-source comparison:** Stacked monthly generation by source.
- **Key insights:** Summary observations about wind generation, seasonal patterns, renewable contributions, and grid flexibility.

## Data Source

The dashboard is based on electricity-market data from **SMARD**, the German Federal Network Agency's market data platform.

- Website: https://www.smard.de/
- Data portal: https://www.smard.de/home/downloadcenter/download-market-data/

The dashboard screenshot shows a selected period from **17 October 2024 to 27 October 2026**, with hourly resolution. Exact coverage and available categories depend on the data included in the project files.

## Data Preparation and Modelling

The project workflow includes:

1. Sourcing electricity-generation time-series data from SMARD.
2. Cleaning and transforming the source data with Power Query.
3. Preparing date/time fields, generation categories, and numerical generation values.
4. Organising the data model for analysis across energy sources and time.
5. Creating DAX measures for headline KPIs, generation totals, and source contributions.
6. Building interactive visuals to explore trends, seasonality, and the electricity mix.

## Suggested Repository Structure

The structure below is a recommended organisation for publishing the project. Adjust the filenames to match the files you actually include.

```text
Germany-Electricity-Generation-Analysis-Dashboard/
│
├── README.md
│
├── assets/
│   └── dashboard-preview.png
│
├── data/
│   ├── raw/
│   │   └── README.md
│   └── processed/
│       └── README.md
│
├── powerbi/
│   └── Germany-Electricity-Generation-Dashboard.pbix
│
├── excel/
│   └── README.md
│
└── docs/
    ├── data-dictionary.md
    └── methodology.md
```

### Folder guide

| Path | Purpose |
|---|---|
| `assets/` | Dashboard screenshots and other project images. |
| `data/raw/` | Original SMARD downloads, where redistribution is permitted. |
| `data/processed/` | Cleaned or transformed datasets used by the report. |
| `powerbi/` | Power BI `.pbix` report file. |
| `excel/` | Supporting Excel workbooks, if used. |
| `docs/` | Data dictionary, methodology, and other documentation. |

## How to Explore the Project

1. Open the `.pbix` file in Microsoft Power BI Desktop.
2. If the report asks for source files, update the Power Query source paths to match your local `data/` directory.
3. Refresh the data, then use the report filters to explore the date range, energy source, resolution, month, and year.
4. Navigate between report pages to review generation trends, the electricity mix, seasonality, and energy-source insights.

> **Note:** The Power BI file and source datasets need to be added to this repository before users can reproduce or refresh the report. The README describes the intended workflow; it does not imply those files are already committed.

## Potential Questions This Dashboard Helps Explore

- How does Germany's electricity generation mix change over time?
- How do onshore and offshore wind generation compare?
- What seasonal patterns appear in wind and solar generation?
- What share of total generation comes from individual energy sources?
- How do renewable and conventional generation sources contribute to the overall mix?

## Data and Usage Notes

- Electricity generation values are presented in **MWh**, as indicated in the dashboard.
- The selected date range and report filters determine the values displayed in the visuals.
- Please consult SMARD's data terms and source metadata when reusing or redistributing downloaded data.
- Dashboard totals and percentages should be interpreted in the context of the selected filters and the underlying source data.

## Author

**Minhazul**

GitHub: [@Minhazul22](https://github.com/Minhazul22)

---

If you find this project useful, feel free to star the repository.
