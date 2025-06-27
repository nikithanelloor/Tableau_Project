# Sample Superstore – Region-Wise Sales Analysis (Tableau)

Analyze and compare sales performance across U.S. regions using the Sample Superstore dataset.

---

##  Project Overview
This Tableau dashboard helps decision-makers:
- Compare **Sales**, **Profit**, **Quantity**, and **Profit Ratio** across **West, East, Central, and South** regions.
- Identify seasonal trends and regional performance using maps, bar charts, and trend lines.
- Drive strategy through interactive exploration and KPI-driven insights.

---

##  Tools & Dataset
- **Tableau Desktop** – For interactive visualizations.
- **Dataset** – Sample Superstore Excel file

 ##  Tasks Performed

1. **Data Source Setup**  
   - Connected Tableau to the Sample Superstore dataset.  
   - Organized dimensions and measures into logical folders: *Categories*, *Order Info*, *Sales*, *Map Data*.

2. **Hierarchy & Parameters**  
   - Created a *Location* hierarchy: Country → Region → State → City.  
   - Added two parameters: **Primary Region** and **Secondary Region** (selectable from all regions).

3. **Region Selection Logic**  
   - Built calculated fields referencing both parameters.  
   - Utilized these to filter and compare data across selected regions.

4. **Geographic Visualization**  
   - Developed a regional/state map using the *State* field.  
   - Added filters driven by region parameters for dynamic map comparison.

5. **Time-Aware Sales Tracking**  
   - Created a *First Order Date* field using Tableau LOD:  
     `{ FIXED [Primary Region]: MIN([Order Date]) }` (and similarly for secondary).  
   - Calculated region-level metrics: Total Sales, Average Sales per Order, Distinct Counts of Customers, Orders, and Products.

6. **Sub-category Analysis**  
   - Designed a cross-tab sheet summarizing Total, Min, and Max Sales by Sub-category.  
   - Complemented with a line chart tracking Sales over time and a bar chart of sub-category performance.

7. **Applied Filters & Final Dashboard**  
   - Applied parameter filters across all sheets to ensure consistency.  
   - Assembled the dashboard: aligned views, partitioned into primary and secondary region panels, and combined maps, charts, and KPIs for side-by-side analysis.
  
## Insights (Region-Wise)
- West leads in both sales and profit, showing it as the highest-performing region.

- East follows closely, with strong sales and solid profits, making it a secondary growth focus. 

- Central region generates high sales but lags in profitability—indicating cost or pricing inefficiencies. 

- South underperforms overall, yet still contributes moderate profit, suggesting room for improvement. 


## Conclusions 
Regional performance varies widely: while the West thrives, the Central region's revenue isn’t translating into proportional profits. Additionally, seasonal trends (e.g., holiday peaks) significantly impact performance across regions.


## Recommendations

- Enhance Profitability in Central Region

- Review pricing, costs, and discount strategies—high revenue needs balanced margin management .

- Focus Expansion in Underperforming Regions

- South and Central show potential; targeted promotions or expanded offerings could yield growth. 

- High holiday sales in November–December can be optimized via staffing and inventory planning 

- Drill Down on Product-Region Profitability

- Identify top performers (e.g., Tables losing despite high sales) and adjust inventory, pricing, or promotional focus accordingly.

  
