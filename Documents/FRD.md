# Functional Requirements Document (FRD)
## Project: E-Commerce Sales Analysis Dashboard

### 1. Data Requirements
- Order ID
- Order Date
- Customer
- Customer Segment
- Category
- Sub-Category
- Product Name
- Quantity
- Price
- Sales
- Profit
- Region

### 2. Cleaning Requirements
- Trim extra spaces
- Fill missing values in Discount with 0
- Convert Order Date into Date type
- Ensure numeric fields are correctly typed

### 3. Dashboard Pages
1. **Overview Page**
   - KPIs: Total Sales, Total Orders, Total Profit, AOV
   - Category-wise sales
   - Region map

2. **Sales Trend Page**
   - Month-over-month sales line chart

3. **Category Insights Page**
   - Sub-category sales comparison
   - Top 10 products

4. **Customer Insights Page**
   - Customer segment sales (pie/donut)
   - Repeat customer metric

### 4. DAX Measures
- Total Sales = SUM(Sales)
- Total Orders = DISTINCTCOUNT(Order ID)
- Total Profit = SUM(Profit)
- AOV = Total Sales / Total Orders
