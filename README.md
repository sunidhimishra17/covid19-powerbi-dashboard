## Covid19-PowerBI-Dashboard

An automated, interactive, and dynamic Power BI dashboard designed to track and analyze global COVID-19 data. This project connects directly to a live data source to ensure real-time reporting without the need for manual data processing or external scripts.

## Features

* **Live Data Connection:** Connected directly to the live [Johns Hopkins University COVID-19 dataset](https://github.com/CSSEGISandData/COVID-19) via Web Connector for automated data refreshes.

* **Interactive Visualizations:** Deep dive into global metrics using interactive maps, slicers, and timelines.

* **Key Metrics Tracked:** Total Confirmed Cases, Active Cases, Recoveries, and Mortality Rates.

* **Trend Analysis:** Time-series charts showing daily/weekly growth trends across different countries and regions.

* **No Code Automation:** Fully built using Power BI's native capabilities, eliminating complex Python/Jupyter data prep bottlenecks.

## Tech Stack & Tools

* **BI Tool:** Power BI Desktop

* **Data Source:** Live CSV/Web API 

* **Data Transformation:** Power Query (M Language)

## Dashboard Insights

The dashboard provides a 360-degree view of the pandemic's impact, including:

1. **Global Summary:** High-level KPIs for quick decision-making.

2. **Country-wise Breakdown:** Compare statistics between different nations seamlessly.

3. **Forecasting & Trends:** Visualizing the curve to understand the trajectory of cases.

## Dashboard Preview

| Main Dashboard | Trend Analysis |
|---|---|
| ![Dashboard Screenshot 1](path-to-your-image1.png) | ![Dashboard Screenshot 2](path-to-your-image2.png) |

## Data Source Credibility

The data used in this project is sourced directly from the **[Johns Hopkins University COVID-19 Dataset](https://github.com/CSSEGISandData/COVID-19)**, which is widely recognized as an official and reliable repository for pandemic tracking.

## Key DAX Measures Used

* **Total Active Cases:**
  '''DAX

      Active Cases = [Total Confirmed] - [Total Recovered] - [Total Deaths]

* **Mortality Rate (%):**

      Mortality Rate = DIVIDE([Total Deaths], [Total Confirmed], 0)

## How to View This Project

1. Clone this repository to your local machine.

2. Open the `covid19-powerbi-dashboard.pbix` file using Power BI Desktop.

3. Click on the Refresh button in the Home ribbon to fetch the latest live data automatically.
