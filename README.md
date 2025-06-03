# Cost Optimization in Manufacturing

This project focuses on analyzing and optimizing manufacturing costs through data analytics and KPI dashboards. It resulted in a 12% reduction in unnecessary expenditures by improving resource allocation and implementing continuous improvement initiatives.

## 📈 Project Overview

- Built a Python-based analytical model to track production costs.
- Used statistical methods and business rules to identify cost drivers and inefficiencies.
- Created interactive KPI dashboards in Power BI to assess cost efficiency across production stages.
- Delivered actionable insights to the operations team, reducing expenses by 12%.

## 🔧 Technologies Used

- Python (pandas, matplotlib, seaborn)
- Power BI
- SQL (for initial data extraction)
- Jupyter Notebook
- Git

## 📁 Project Structure

Clone this repo:

2. Install dependencies:

3. Open the notebook:

4. To view the dashboard, open `cost_kpi_dashboard.pbix` in Power BI Desktop.

## 📊 Results

- Identified underutilized machines and overstaffed shifts.
- Streamlined material procurement schedules.
- Enabled data-driven decisions with real-time KPIs.

## 📬 Contact

For questions or collaboration:
- 📧 your.email@example.com
- 🌐 [LinkedIn](https://www.linkedin.com/in/your-profile)

pandas
matplotlib
seaborn
jupyter
import pandas as pd

# Load data
df = pd.read_csv('../data/production_costs.csv')

# Basic analysis
df['Total_Cost'] = df['Material_Cost'] + df['Labor_Cost'] + df['Overhead']

# Identify cost outliers
high_cost = df[df['Total_Cost'] > df['Total_Cost'].quantile(0.95)]
print("High-cost production batches:")
print(high_cost[['Batch_ID', 'Total_Cost']])
