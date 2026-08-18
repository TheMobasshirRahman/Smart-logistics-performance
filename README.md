# Smart Logistics Performance & Delay Analytics

A portfolio-ready data analytics project combining **Python EDA** and an **interactive Power BI dashboard** to analyze logistics delays.

## Project objective

The project investigates operational delay patterns across:

- Shipment status
- Traffic conditions
- Logistics assets
- Day of week
- Hour of day
- Waiting time
- Inventory
- Asset utilization

## Tech stack

| Tool | Purpose |
|---|---|
| Python | Data cleaning, EDA and visualization |
| Pandas / NumPy | Data manipulation |
| Matplotlib | Exploratory charts |
| Power BI | Interactive dashboard and KPI reporting |
| DAX | Measures and business metrics |
| Git / GitHub | Version control and portfolio presentation |

## Dataset

The project uses a 1,000-record logistics dataset. The source contains 16 original columns. A cleaned/enriched version is provided in `data/logistics_data_cleaned.csv`.

`Logistics_Delay` is the binary delay flag:
- `0` = No delay
- `1` = Delay

The original dataset contains missing values in `Logistics_Delay_Reason`; these are retained because missingness can itself be meaningful when a record has no stated delay reason.

## Repository structure

```text
smart-logistics-performance/
│
├── data/
│   ├── logistics_data_cleaned.csv
│   └── data_dictionary.csv
│
├── notebooks/
│   └── smart_logistics_analysis.ipynb
│
├── powerbi/
│   └── DAX_measures_and_visual_plan.txt
│
├── images/
│   └── dashboard screenshots
│
├── README.md
└── requirements.txt
```

## Key dashboard KPIs

- Total Records
- Delayed Records
- Delay Rate
- Average Asset Utilization

## Power BI dashboard

The final Power BI page should contain:

1. KPI cards
2. Shipment status slicer
3. Day slicer
4. Delay status slicer
5. Asset slicer
6. Traffic status slicer
7. Shipment Status Distribution
8. Delay Rate by Traffic Condition
9. Overall Delay Distribution
10. Day-wise Delay Rate
11. Asset-wise Delay Rate
12. Hourly Delay Pattern

A Reset button should return slicers to the default state using a bookmark.

## How to reproduce

### Python / Google Colab

1. Upload the repository to Google Colab.
2. Open `notebooks/smart_logistics_analysis.ipynb`.
3. If necessary, update the data path to the uploaded CSV.
4. Run all cells.
5. Review the KPI and analytical outputs.

### Power BI Desktop

1. Import `data/logistics_data_cleaned.csv`.
2. Set `Timestamp` to Date/Time.
3. Set numeric fields to appropriate numeric types.
4. Create the DAX measures from `powerbi/DAX_measures_and_visual_plan.txt`.
5. Build the dashboard using the recommended visual layout.
6. Add slicers and a Reset bookmark.
7. Save the final `.pbix` locally.
8. Export a dashboard screenshot to `images/`.

## Portfolio talking points

> Built an end-to-end logistics analytics solution using Python and Power BI to identify operational delay patterns and asset-level risk.

> Performed data-quality validation, feature engineering and exploratory analysis using Pandas and NumPy.

> Designed an interactive Power BI dashboard with KPI cards, slicers, DAX measures and operational drill-downs.
