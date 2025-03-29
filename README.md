# Sales Performance

### Dashboard Link : https://github.com/ashokkumarlourthuraj/Sales-Performance-Analysis/blob/main/Sales%20Performance%20%20Analysis.pbix
## Problem Statement

Businesses need a robust and interactive way to analyze sales data for strategic decision-making. The lack of a centralized, automated reporting system leads to inefficiencies in tracking key performance metrics such as revenue, profit, and sales trends. Additionally, manual data handling increases the risk of errors, delays, and inconsistencies in reporting.

This project aims to develop an interactive Sales Performance Dashboard in Power BI that consolidates sales data from multiple sources, automates data loading, and provides insightful visualizations for informed decision-making


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a xlsworksheet file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed Check for duplicates, missing values, and incorrect data types in the dataset.
- Step 5 :Convert the Date column to Date format to enable proper time-based analysis.
- Step 6 : Create a new column for Year using the formula YEAR(Sales[Date]) to analyze trends over time.
- Step 7 : Standardize category names by trimming spaces, converting text to lowercase/uppercase, and replacing inconsistent values
- Step 8 : Remove unnecessary columns to optimize performance and keep only relevant data
- Step 9 : Apply all transformations and load the cleaned dataset for further analysis. 
- Step 10 : In the report view, under the view tab, theme was selected.  
- Step 11 : Define essential calculations using DAX:

Total Sales → Total_Sales = SUM(Sales[Revenue])

Total Profit → Total_Profit = SUM(Sales[Profit])

Profit Margin % → Profit_Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Revenue]))

Year-over-Year Growth → YoY_Growth = (Current Year Sales - Previous Year Sales) / Previous Year Sales

Top-Selling Products & Regions → Using TOPN function

 
 # Report Snapshot (Power BI DESKTOP)

 
![Image](https://github.com/user-attachments/assets/c80d9dce-80aa-4538-8909-25a6dc04fdd3)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### Overall Sales Performance
Total revenue over the years: $87.05M

Total gross profit: $60.02M

Total units sold: 3M

Sales increased steadily from 2014 to 2016.

### Sales Breakdown by Product Category
Extra and Special categories contributed nearly 50% each to total revenue.

Among subcategories, Super performed the best.

### Top Sales Representatives
The highest sales were recorded by
 El Bob  
 Ellen Woody
 Ellie Gill
 Jan Novotny
 John White.

### Quarterly and Monthly Trends
Highest revenue in 2016: $76.19M.

MoM (Month-over-Month) Profit Analysis:

The highest gross profit was recorded in March 2015.

August consistently showed a decline, possibly due to seasonal effects.

### Discounts and Revenue Impact
Discounts were mostly applied to Magnum, Quad, Carlota, Bing, Linder, and VanHelen.

The impact of discounts on revenue remained consistent across subcategories.

### Year-over-Year Revenue Growth
Revenue increased in 2015 and 2016 but saw QoQ (Quarter-over-Quarter) declines 

The best YoY (Year-over-Year) growth was 11.77% in 2015.

### Average Sales Revenue Trends
Highest average revenue per transaction was observed on March 19, 2016 ($3,064.55).

Lowest was on May 1, 2015 ($1,711.43).

### Profitability Trends
Gross profit was highest in each year.

July and October were the most profitable months, while February and August saw lower profits.
