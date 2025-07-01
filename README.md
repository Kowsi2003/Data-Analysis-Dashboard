# ☕ Coffee Sales Data Analysis Dashboard

## 🎯 Project Objective
Build a dynamic, interactive Excel dashboard that transforms raw order data into actionable insights. Stakeholders can filter by date, product, geography, and customer to uncover sales trends, identify top markets, and spotlight high-value accounts.

## Dataset used
- <a href="https://github.com/Kowsi2003/Data-Analysis-Dashboard/blob/main/coffeeOrdersData.xlsx">Coffee Sales Data</a>

## 📊 Key Performance Indicators
- What is our total sales revenue for the selected period?  
- How many orders did we process in that timeframe?  
- What is the average spend per order (Average Order Value)?  
- What percentage of customers are making repeat purchases?  
- How many new customers did we acquire this period?  
- Which product category (roast/variety/size) drove the highest volume? 
- Which country or region contributed the most to our top-line?  
- What overall profit margin did we achieve?  

## Dashboard Interaction <a href="https://github.com/Kowsi2003/Data-Analysis-Dashboard/blob/main/Dashboard.png">View Dashboard</a>

## 🚀 Project Process
1. **Data Collection**  
   - Gather raw CSV files: `orders.csv`, `customers.csv`, `products.csv`.  
   - Store them in the `data/` folder of the repo.

2. **Data Cleaning & Enrichment**  
   - Use Power Query (or Excel formulas) to trim whitespace, correct data types, and remove duplicates.  
   - Merge the tables:  
     - Join `orders` → `customers` on `CustomerID` to pull in name, country, loyalty status.  
     - Join the result → `products` on `ProductID` to add roast, variety, size, unit price, unit cost.

3. **Data Modeling**  
   - Load enriched Orders table into the Excel Data Model (Power Pivot).  
   - Define relationships and create DAX measures for key metrics:  
     - Total Revenue, Profit, Order Count, Repeat Rate, etc.

4. **Dashboard Design**  
   - Insert PivotTables/Charts linked to the Data Model.  
   - Add Timeline control for date filtering.  
   - Add Slicers for Roast Type, Coffee Variety, Size, Loyalty Card.  
   - Arrange KPI cards at the top showing your core metrics.

5. **Visualization & Formatting**  
   - Configure chart types: line charts for trends, bar charts for rankings.  
   - Apply consistent styling (colors, fonts, data labels) for clarity.  
   - Enable interactive filtering so all visuals update together.

6. **Testing & Validation**  
   - Cross-check totals against raw data.  
   - Verify slicers and timeline filters work as expected.  
   - Ensure measures and margins calculate correctly under different scenarios.

7. **Deployment**  
   - Save and commit `coffeeOrdersData.xlsx` with all connections intact.  
   - Push final workbook and README to GitHub.  
   - Share the repo link for reviewers and recruiters to explore.

## Dashboard
![Dashboard](https://github.com/user-attachments/assets/908fbaae-90f8-4672-9c46-f92a95a5b8c2)




