🛣️ Road Accident Analysis Dashboard


The Road Accident Analysis Dashboard provides an interactive Power BI visualization of road safety data, focusing on casualties and accidents across the United Kingdom. It helps stakeholders, policymakers, and data analysts understand key trends in road accidents, identify high-risk areas, and analyze the impact by vehicle type, road type, and location.

🎯 Objectives

Analyze total casualties and accident counts for the current year (CY) vs. previous year.

Visualize the distribution of casualties by road type, vehicle type, and area (urban/rural).

Identify geographical accident hotspots using an interactive map.

Evaluate year-over-year (YoY) performance to assess improvements in road safety.

📈 Key Insights

Total CY Casualties: 196K (↓11.9% YoY)

Total CY Accidents: 144K (↓11.7% YoY)

Fatal Casualties: 3K (↓33.3%)

Serious Casualties: 30K (↓16.2%)

Slight Casualties: 166K (↓10.6%)

Breakdown by Category

By Vehicle Type: Cars, bikes, vans, buses, and agriculture vehicles.

By Road Type: Single and dual carriageways, roundabouts, one-way streets, slip roads.

By Area: Urban vs. rural distribution.

By Month: CY vs. PY casualty trends visualized in a monthly line chart.

🗺️ Dashboard Features

Dynamic KPIs: Key metrics update based on selected filters.

Time Comparison: Visual comparison of CY vs. PY monthly casualties.

Geospatial Map: Accident distribution across UK regions.

Interactive Filters: Drill down by road type, vehicle type, and region.

Data Cards & Pie Charts: Summarize critical accident information at a glance.

🧠 Tools & Technologies

Data Visualization: Microsoft Power BI

Data Source: UK Department for Transport — Road Accident Data

Data Cleaning & Modeling: Power Query, DAX

Measures Used:

CY Casualties = TOTALYTD(SUM(Data[Number_of_Casualties]), Calendar[Date])
PY Casualties = CALCULATE(SUM(Data[Number_of_Casualties]), SAMEPERIODLASTYEAR(Calendar[Date]))
YOY Casualties = ([CY Casualties] - [PY Casualties]) / [PY Casualties]


Map Visual: Bing Map / Azure Maps

📂 Files in Repository
📁 Road_Accident_Analysis/
│
├── power.pbix      # Power BI dashboard file
├── Road Accident Data.csv                         # Cleaned dataset (if included)
├── README.md                        # Documentation (this file)
└──road.png
   

🚦 How to Use

Download the .pbix file.

Open it in Power BI Desktop.

If prompted, connect or refresh the dataset source path.

Explore the interactive visuals, apply filters, and analyze trends.

💡 Future Improvements

Integrate live data updates via API.

Add forecasting and predictive models for accident trends.

Include weather and traffic correlation analysis.

Deploy Power BI Service dashboard with auto-refresh.


