# Pivot Table Guide for Bikes Dekho Sales Analysis

## What is a Pivot Table?
A pivot table is an Excel feature that automatically summarizes and analyzes large datasets. It allows you to quickly reorganize and group data to gain new insights.

## Creating Your First Pivot Table

### Step 1: Select Your Data
1. Click on any cell in your data range
2. Go to **Insert** > **PivotTable**
3. Excel automatically detects the data range
4. Click **OK** to proceed

### Step 2: Arrange Fields
The Pivot Table Field List appears on the right side with four areas:

#### Filters (Top)
- Drag fields here to filter entire pivot table
- Use for: Region, Year, Category

#### Columns
- Drag fields here to create column headers
- Use for: Gender, Education, Product Type

#### Rows
- Drag fields here to create row headers
- Use for: Age Group, Region, Customer Segment

#### Values
- Drag fields here to calculate summaries
- Use for: Sum of Revenue, Count of Records, Average Price

## Common Pivot Table Examples

### Example 1: Revenue by Region and Gender
```
Rows: Region
Columns: Gender
Values: Sum of Sale_Amount
```
This creates a grid showing:
- Each region in rows
- Male/Female in columns
- Total revenue at intersections

### Example 2: Customer Count by Age Group and Income
```
Rows: Age_Group, Income_Level
Columns: (empty)
Values: Count of Customer_ID
```
Results in hierarchical view:
- Age groups in main rows
- Income levels as sub-rows
- Customer count in values

### Example 3: Sales Trend Over Time
```
Rows: Month, Year
Columns: Product_Category
Values: Sum of Quantity, Average of Price
```
Shows multiple value types side-by-side

## Calculating Values

### Common Aggregation Functions
1. **Sum**: Total of all values
   - Use for: Revenue, Quantity, Total sales
   
2. **Count**: Number of records
   - Use for: Customer count, Transaction count
   
3. **Average**: Mean value
   - Use for: Average price, Average rating
   
4. **Min/Max**: Smallest/largest value
   - Use for: Price range, Score distribution
   
5. **Distinct Count**: Unique values (Excel 2013+)
   - Use for: Unique customers, Unique products

### Changing Value Calculations
1. Double-click the value field in the Pivot Table
2. Choose new function from list
3. Click **OK**

## Filtering Pivot Table Data

### Using Row/Column Filters
1. Click dropdown arrow on field name
2. Uncheck items to hide them
3. Check items to show them
4. Click **OK**

### Using Report Filters
1. Drag field to "Filters" area
2. Dropdown appears at top of pivot table
3. Select filter criteria
4. Pivot table updates automatically

## Formatting & Styling

### Change Number Formats
1. Right-click on value cell
2. Select **Format Cells**
3. Choose format: Currency, Percentage, etc.
4. Click **OK**

### Apply Design Styles
1. Click anywhere in pivot table
2. Go to **Design** tab
3. Choose style from **PivotTable Styles**
4. Automatically formats entire table

### Adjust Column Widths
1. Double-click column border to auto-fit
2. Or drag border to manual width
3. All columns auto-adjust together

## Advanced Features

### Sorting
1. Click field dropdown arrow
2. Select **Sort A to Z** or **Sort Z to A**
3. Or sort by values: **More Sort Options**

### Grouping
1. Right-click on row label
2. Select **Group**
3. Choose grouping criteria:
   - By months/years for dates
   - By ranges for numbers
   - By selection for text

### Slicers
1. Click pivot table
2. Go to **Insert** > **Slicer**
3. Select fields to slicer
4. Click **OK**
5. Click buttons on slicer to filter

### Calculated Fields
1. Go to **Analyze** > **Fields, Items & Sets**
2. Select **Calculated Field**
3. Name the field and enter formula
4. Click **OK**

Example: Profit Margin
```
= Revenue / Cost - 1
```

## Troubleshooting Common Issues

### Pivot Table Won't Refresh
- Right-click pivot table
- Click **Refresh**
- Or: Ctrl+A in pivot, then Refresh

### Data Not Showing
- Check if field is in correct area
- Verify data range is correct
- Ensure source data is updated

### Incorrect Calculations
- Verify value function (Sum, Count, etc.)
- Check for text values in numeric columns
- Remove filters if needed

### Pivot Table Too Large
- Add filters to reduce data
- Move fields to different areas
- Create separate pivot tables by category

## Tips for Better Pivot Tables

✅ **Use consistent data types** - Don't mix text and numbers
✅ **Include headers** - Label every column in source data
✅ **Use meaningful names** - Make column names clear and descriptive
✅ **Keep source data clean** - Remove duplicates before pivoting
✅ **Create backups** - Save before major pivot table changes
✅ **Use named ranges** - Makes pivot tables easier to manage
✅ **Document calculations** - Note what each value represents
✅ **Update regularly** - Refresh after source data changes

## Dashboard Integration

### Connect Slicers
1. Create multiple pivot tables
2. Insert slicers on one
3. Right-click slicer
4. Select **Report Connections**
5. Check other pivot tables
6. Now slicer filters all connected tables

### Embed in Dashboard
1. Format pivot table professionally
2. Copy and paste into dashboard sheet
3. Link with slicers
4. Add title and description
5. Set to refresh with data update

## Performance Tips

### For Large Datasets (>100k rows)
- Use filtering to reduce data size
- Create separate pivot tables by category
- Store in separate sheet
- Consider data model for analysis

### Improving Pivot Table Speed
- Remove unused fields
- Limit filter options
- Use fewer calculated fields
- Archive historical data

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| Alt+D,P,T | Insert pivot table |
| Ctrl+A | Select all in pivot |
| F5 | Go to cell |
| Ctrl+R | Refresh pivot table |

## Resources

- **Excel Help**: F1 then search "pivot table"
- **Microsoft Docs**: office.com/pivot-tables
- **Training**: LinkedIn Learning Excel courses

---

For detailed analysis examples, see `Data_Analysis_Guide.md`
