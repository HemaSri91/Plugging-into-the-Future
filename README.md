⚡ Plugging into the Future
An Exploration of Electricity Consumption Patterns Using Tableau

📌 Project Overview
Plugging into the Future is a data visualization project built using Tableau to analyze electricity consumption patterns across different regions, sectors, and seasons.
This project transforms raw electricity usage data into interactive dashboards that provide meaningful insights for:

⚡ Utility Companies
🏛 Policymakers
🏭 Energy Planners
👥 Consumers
The goal is to optimize electricity usage, improve grid reliability, and support sustainable energy planning.

📊 Project Scenarios
🔹 1. Time-of-Day Usage Patterns
   Identify peak and off-peak demand hours
   Analyze hourly electricity consumption trends
   Support time-of-use pricing strategies
🔹 2. Seasonal Variations & Forecasting
   Analyze monthly and seasonal usage fluctuations
   Detect demand spikes during summer/winter
   Use Tableau forecasting to predict future demand
🔹 3. Sector-Specific Consumption Insights
   Compare Residential, Commercial, and Industrial usage
   Identify highest energy-consuming sectors
   Support targeted energy efficiency programs

📁 Dataset
File Used: Consumption.csv
Sample Fields:
Date
Hour
Region
Sector
Consumption (kWh/MW)

🛠 Tools & Technologies

📊 Tableau Desktop / Tableau Public
📁 CSV Dataset
🌐 HTML (for GitHub Pages deployment)
🎨 Tailwind CSS (Website Styling)

📈 Key Performance Indicators (KPIs)

Total Electricity ConsumptionPeak Demand Hour
Highest Consuming Region
Highest Consuming Sector
Seasonal Growth Rate (%)
Forecasted Demand

🧮 Tableau Calculated Fields
Season Classification
IF MONTH([Date]) IN (3,4,5,6) THEN "Summer"
ELSEIF MONTH([Date]) IN (7,8,9) THEN "Monsoon"
ELSE "Winter"
END
Peak Indicator
IF SUM([Consumption]) > WINDOW_AVG(SUM([Consumption])) 
THEN "Peak"
ELSE "Normal"
END

🖥 Dashboard Features

📊 Line Charts (Hourly & Monthly Trends)
🔥 Heatmaps (Peak Load Visualization)
📌 Bar Charts (Sector Comparison)
📈 Forecast Models

🎛 Interactive Filters (Region, Sector, Date)
