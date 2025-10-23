# Road-Accident-Data-Analysis

# Problem Statement

## The Clients wants to create a Road Accident Dashboard for year 2021 and 2022 so that they can have insight on the below requirements
     Primary KPI - Total Casualties taken place after the accident
     Primary KPI's - Total Casualties & percentage of total with respect to accident severity and maximum casualties by type of vehicle
     Secondary KPI's - Total Casualties with respect to vehicle type
     Monthly trend showing comparison of casualties for Current Year and Previous Year
     Maximum casualties by Road Type
     Distribution of total casualties by Road Surface

### 🔍 Step 1: Understand the Dataset
### Firstly, I’ll took a quick look at the structure of your Excel file — specifically:
     What sheets are present.
     What columns exist (e.g., Year, Month, Accident_Severity, Vehicle_Type, Casualties, Road_Type, etc.).
     This will allow me to map the data fields to your KPIs.
     Cleeaned the data by extrating days, Months and Year from the dates Using the below formulae:
          =TEXT(B2,"DD")
          =TEXT(B2,"MMM")
          =TEXT(B2,"YYYY")

### Step 2: Dashboard Metrics Design
### Primary KPIs
     Total Casualties
     Formula: =SUM(Casualties)
### Card visualization
     Casualties by Accident Severity
     Severity categories: Fatal, Serious, Slight
     Show total and % of total using:
     =F9/($F$9 +$F$10) i.e (Casualties by Severity) / (Total Casualties)

### Max Casualties by Vehicle Type
     Pivot Table: Vehicle Type vs SUM of Casualties
     Highlight maximum value.
     Visualization: Pie chart 

### Secondary KPIs
     Total Casualties by Vehicle Type
     Visualization: Pie chart

### Step 3: Trends and Comparisons
     Monthly Trend Comparison (2021 vs 2022)
     Pivot: Month as Axis, SUM(Casualties) as Values, Year as Legend.
     Visualization: Line chart with two lines (2021 and 2022)

### Step 4: Contextual Insights
     Max Casualties by Road Type
     Pivot: Road Type by count(Casualties) using Calculated items
     Visualization: Bar Chart.

	 Distribution by Road Surface
     Pivot: Road Surface × count(Casualties)
     Visualization: Hierarachy Chart.
     Casualties by Area and Time (Day/Night)

	Pivot: Rows → Area/Location; Columns → Day/Night; Values → SUM(Casualties)
	Visualization: Pie Chart

### Dashboard
																
<img width="1868" height="785" alt="image" src="https://github.com/user-attachments/assets/94799f7b-c52b-48bd-95b5-bd3eb4229c32" />



     

    
