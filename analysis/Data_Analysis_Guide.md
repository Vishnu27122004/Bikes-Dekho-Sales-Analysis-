# Bikes Dekho Sales Analysis - Data Analysis Guide

## Overview
This guide provides step-by-step instructions for analyzing the Bikes Dekho sales data using Excel.

## Data Cleaning & Preparation

### Step 1: Load Raw Data
1. Open `Raw_Data.xlsx`
2. Review the data structure and identify columns
3. Check for missing values and inconsistencies

### Step 2: Data Validation
- Remove duplicate records
- Standardize date formats (MM/DD/YYYY)
- Ensure consistent data types for each column
- Validate numerical ranges for key metrics

### Step 3: Feature Engineering
- Create Age Groups: 18-25, 26-35, 36-45, 46-55, 55+
- Create Income Categories: Low, Medium, High
- Create Commute Categories: Short (<5km), Medium (5-15km), Long (>15km)

## Creating Pivot Tables

### Revenue Analysis Pivot Table
1. Select cleaned data
2. Insert → Pivot Table
3. Rows: Region, Gender
4. Columns: Education Level
5. Values: Sum of Sale Amount

### Customer Segmentation Pivot Table
1. Rows: Age Group, Income Level
2. Columns: Commute Type
3. Values: Count of Customer ID

### Time-based Analysis Pivot Table
1. Rows: Month, Year
2. Columns: Product Category
3. Values: Sum of Quantity, Average of Price

## Dashboard Creation

### Step 1: Set Up Dashboard Sheet
1. Create new sheet: "Dashboard"
2. Add title and date range
3. Leave space for charts and KPI cards

### Step 2: Add KPI Cards
```
Total Revenue =SUMALL(Sales)
Total Customers = COUNTA(Customer_IDs)
Average Order Value = Revenue / Orders
Customer Satisfaction = AVERAGE(Ratings)
```

### Step 3: Create Visualizations
- Revenue by Region (Column Chart)
- Customer Distribution by Gender (Pie Chart)
- Sales Trend (Line Chart)
- Top Products (Bar Chart)

### Step 4: Add Interactive Slicers
1. Select pivot table
2. Insert → Slicer
3. Add slicers for: Region, Gender, Age Group, Education

## Key Analyses

### Revenue Analysis
1. **By Region**: Which regions generate most revenue?
2. **By Customer Segment**: High-value vs low-value segments
3. **By Product**: Most popular and profitable products
4. **By Time**: Seasonal trends and growth patterns

### Customer Analysis
1. **Demographics**: Age, gender, income distribution
2. **Behavior**: Purchase frequency, average transaction value
3. **Loyalty**: Repeat purchase rates
4. **Segmentation**: Cluster customers by value

### Geographic Analysis
1. **Regional Performance**: Revenue, customer count, growth
2. **Market Penetration**: Untapped opportunities
3. **Regional Trends**: Local preferences and patterns

## Advanced Analysis

### Correlation Analysis
```
= CORREL(Income, Purchase_Amount)
= CORREL(Age, Product_Category)
= CORREL(Education, Average_Order_Value)
```

### Trend Analysis
```
= FORECAST(next_period, historical_data)
= TREND(Sales_Data, Period_Data)
```

### Segmentation Analysis
1. Use conditional formatting to identify segments
2. Create segment profiles
3. Calculate segment metrics

## Report Generation

### Executive Summary
- Key findings in 1-2 pages
- Top 3-5 insights
- Recommendations

### Detailed Analysis Report
1. Revenue Analysis (2-3 pages)
2. Customer Analysis (2-3 pages)
3. Geographic Analysis (1-2 pages)
4. Segment Analysis (2-3 pages)
5. Recommendations (1-2 pages)

## Tips & Tricks

### Excel Shortcuts
- Ctrl+Shift+V: Paste Special
- Ctrl+G: Go To
- F4: Toggle absolute/relative references
- Ctrl+`: Toggle formula view

### Common Formulas
```
=SUMIFS(sum_range, criteria_range, criteria)
=COUNTIFS(count_range, criteria)
=AVERAGEIFS(average_range, criteria_range, criteria)
=INDEX(array, MATCH(lookup_value, lookup_array, 0))
```

## Troubleshooting

### Pivot Table Issues
- **Table not updating**: Right-click → Refresh
- **Missing data**: Check source data range
- **Formatting issues**: Drag fields to correct areas

### Chart Issues
- **Chart not displaying**: Check data range
- **Legend problems**: Use "Switch Row/Column"
- **Scale issues**: Adjust axis minimum/maximum

## Data Refresh Workflow

1. Update source data in Raw_Data sheet
2. Refresh all pivot tables (Ctrl+A in pivot, then Refresh)
3. Charts auto-update automatically
4. Dashboard reflects latest data
5. Export reports as PDF

## Best Practices

✅ Always work with a backup copy
✅ Use consistent naming conventions
✅ Document your formulas with comments
✅ Keep pivot tables organized by topic
✅ Use data validation for input cells
✅ Format data clearly for readability
✅ Test formulas before finalizing
✅ Update dashboards monthly

## Resources
- Excel Help: F1
- Pivot Table Guide: Insert → Recommended Pivot Tables
- Chart Wizard: Insert → Recommended Charts

---
For questions or issues, refer to the main README or create an issue on GitHub.
