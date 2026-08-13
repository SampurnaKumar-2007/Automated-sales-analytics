# Automated-sales-analytics
An automated Python (Extract. Transform, load)ETL data pipeline that ingests raw transactional sales data, performs cleaning and aggregation with Pandas, and exports multi-tab Excel executive reports.

## Key Technical Features

Uses NumPy to generate 500+ transactional records with realistic probabilities and controlled missing values (`np.nan`).
Resolves missing numerical quantities using median imputation to handle discrete order counts and mean imputation for continuous metrics like customer ratings.
Derives line-item metrics including `Total_Revenue` (`Units_Sold` × `Unit_Price`) and standardizes time-series strings into structured datetime objects (`YYYY-MM`).
Groups data across multiple dimensions (**Product Category** and **Region**) to aggregate total order volumes, units sold, total revenue, and average ratings.
Uses `openpyxl` engine via Pandas to programmatically build an **Executive Summary** dashboard with custom row spacing alongside a full **Cleaned Data** audit tab.

---

## Tech Stack & Libraries

* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Excel Engine:** OpenPyXL
* **Development Environment:** Google Colab

---

## Repository Structure

* `automated_sales_analytics.ipynb` – Complete Python script and execution notebook.
* `raw_sales_data.csv` – Ingested raw dataset featuring generated transactional logs.
* `Automated_Sales_Report.xlsx` – Multi-tab Excel report generated automatically by the pipeline execution.

