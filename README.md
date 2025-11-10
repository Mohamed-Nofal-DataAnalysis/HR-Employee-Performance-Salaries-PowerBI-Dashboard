# HR Employee Performance & Salaries Interactive Dashboard
**(Built 100% in Power BI)**
## Project Objective
Create a fully interactive Power BI dashboard for **"Technology Your Text"** that analyzes employee salaries, performance ratings, and distribution across locations, departments, and positions — with real-time filtering via slicers to optimize HR strategies and boost efficiency!
## Dataset Used
[Download Full Dataset (excel files)](https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/tree/main/Dateset)
## Questions (KPIs) Answered Instantly
- Total Employees = 94 | Low Performers = 51 across departments
- Total Salary Expenditure = $1.2M | Avg Performance Rating = 15
- Year-over-Year Change = -1% in performance
- Top Department by Salary = Sales → $510.2K (42.5% of total)
- Top Position by Cost = Sales Rep → $475.2K
- Employee Distribution by Department (Donut + Bar)
## Dashboard Interaction (Click any slicer → everything updates live)
[Detailed Insights](https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Detailed_Insights.png) | [Performance Across Locations](https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Performance_Across_Locations.png) | [Salaries Analysis](https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Salaries_Analysis.png)
## Process (Pro Level – Step by Step)
1. **Data Collection** → 4 tables (Employees, Salaries, Performance, Locations/Departments)
2. **Data Cleaning** → Power Query (removed duplicates, fixed data types, filled nulls)
3. **Data Modeling** → Star Schema + Active Relationships
4. **DAX Measures** →
   ```dax
   Total Employees = COUNTROWS(Employees)
   Total Salary = SUM(Salaries[Amount])
   Avg Rating = AVERAGE(Performance[Rating])
   YoY Change % = DIVIDE([Total Salary] - CALCULATE([Total Salary], PREVIOUSYEAR('Date'[Date])), CALCULATE([Total Salary], PREVIOUSYEAR('Date'[Date])))
   Profit % = DIVIDE([Total Profit], [Total Revenue])
## Interactive Slicers :
 Department, Location, Position, Year
## Visuals :
Line Chart, Donut Chart, Bar Chart, KPI Cards, Funnel Chart, Icons
## Design :
Warm pastel theme + HR icons + custom tooltips
## Dashboard Screenshots (Click to enlarge)
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Detailed_Insights.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Performance_Across_Locations.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Salaries_Analysis.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/HR-Employee-Performance-Salaries-Power-BI-Dashboard/blob/main/Modeling.png">
## Key Insights That Will Change Your Strategy
Sales department dominates with $510.2K salary spend
51 low performers identified → target training in Marketing & Sales!
-1% YoY decline in ratings (visible in line chart from 2000-2020)
Only 3 departments (Sales, Marketing, Admin) = 100% employees → focus retention there
Sales Rep & Marketing Manager = high cost positions → review compensation or automate
## Final Conclusion :
This isn’t just a report… it’s a real-time HR optimization machine.
One click on any slicer and you instantly see where to invest in training, where to cut costs, and which department deserves a performance bonus!
