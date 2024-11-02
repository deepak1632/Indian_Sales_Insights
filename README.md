# India Sales Insights Dashboard

### Dashboard Link: [Power Bi Dashboard](https://app.powerbi.com/groups/me/reports/1fa24168-3851-47d3-8ce9-f65c354b5fd9/a2b94f593e92c9542a94?experience=power-bi)

## Problem Statement

This dashboard provides a comprehensive overview of sales trends across India from 2017 to 2020, enabling analysts and decision-makers to understand sales performance, revenue generation, and profit distribution across various regions and product categories. By identifying key sales metrics such as revenue growth, profit margins, and sales quantities, businesses can make data-driven decisions to optimize strategies and maximize profitability.

The dashboard highlights both strong and underperforming areas, allowing stakeholders to pinpoint areas for improvement and focus resources effectively. With Power BI’s interactive filtering, users can drill down by region, product category, and year, making it an invaluable tool for strategic planning and operational enhancements.

### Steps Followed

- **Step 1**: Imported data files containing historical sales statistics (2017–2020).
  
- **Step 2**: Cleaned and standardized currency formats and removed duplicates in SQL, followed by additional data cleaning within Power BI.
  
- **Step 3**: Loaded the cleaned data into Power BI for further analysis and visualization.

- **Step 4**: Performed data profiling in Power BI to assess data quality, check for missing values, and validate column formats.
  
- **Step 5**: Addressed null values in fields like "Profit Margin %" and "Revenue Contribution %" to ensure they didn't affect analysis accuracy.

- **Step 6**: Added visual filters (Slicers) for fields such as "Region," "Product Category," and "Year" to allow for focused insights.

- **Step 7**: Key performance metrics including "Overall Revenue," "Profit Margin %," and "Revenue Contribution %" were visualized through custom visuals.

- **Step 8**: Bar charts illustrated revenue and profit distribution by region and product category, with segmentation by year and product type.

- **Step 9**: Summary cards displayed high-level metrics such as overall revenue and profit margin, providing a quick snapshot of performance.

- **Step 10**: Detailed analysis of revenue and profit trends across categories and regions, enabling identification of high and low-performing segments.

### Steps for Data Refinement in Power BI

- **Step 11**: Created calculated columns to categorize regions and products based on their contribution to revenue and profitability.

- **Step 12**: Developed measures for key sales metrics, including Total Revenue, Profit Margin %, and Revenue Contribution %, to enrich insights.

- **Step 13**: Added dynamic filters, allowing users to refine insights based on specific parameters such as product category, region, and year.

### DAX Expressions

- **Total Revenue** = SUM(Sales_Data[Revenue])
  
- **Profit Margin %** = DIVIDE(SUM(Sales_Data[Profit]), SUM(Sales_Data[Revenue])) * 100
  
- **Revenue Contribution %** = DIVIDE(SUM(Sales_Data[Revenue]), CALCULATE(SUM(Sales_Data[Revenue]), ALL(Sales_Data[Product_Category])))

### Key Insights
- **Total Sales Period Analyzed**: 2017 to 2020

1. **Top Performers:**
   - The top revenue-generating regions and product categories were identified, highlighting areas of high profitability.

2. **Revenue Insights:**
   - Annual Revenue Growth Rate
   - Key Product Categories: Electronics and Fashion

3. **Profitability Analysis:**
   - **Overall Profit Margin**: 15.8%
   - Highest Profit Margin by Region: North India

4. **Sales Quantity Trends:**
   - Increasing demand in certain categories, especially in South India.

### Visualizations and Analysis

1. **Bar Chart**: Compares total revenue by region and product category over time.
  
2. **Line Chart**: Shows annual revenue and profit trends, helping to identify peaks and dips.

3. **Pie Chart**: Breakdown of revenue contribution by region, showcasing which regions contribute the most to overall revenue.

4. **Custom Visuals**: Display key sales metrics like "Revenue Contribution %" and "Profit Margin %" for easy comparison.
   
6. **Summary Cards**: Display overall metrics like Total Revenue (₹985M), Total Sales Quantity (2M), and Overall Profit Margin.

7. **Top 5 Customers and Products**: Separate visuals highlight top customers and products based on revenue, aiding in product and customer prioritization.

### Report Snapshot (Power BI DESKTOP)

![Screenshot 2024-10-28 064327](https://github.com/user-attachments/assets/1f495fe2-493b-47d7-bc0a-92c40a30b074).

![Screenshot 2024-10-28 063735](https://github.com/user-attachments/assets/7fe68ead-5f5f-4673-bb70-b7cfd9385e4b)

### Insights

1. **Revenue Trends**:
   - North India and Electronics lead in revenue contribution, indicating high consumer demand in this region and product category.
   - Annual peaks in the festive season drive significant revenue spikes.

2. **Profit Margin Analysis**:
   - Product categories with high-profit margins contribute significantly to overall profitability, with a focus on luxury goods.

3. **Sales Volume**:
   - Higher sales quantities are linked to discounts and promotions, especially in peak seasons.
