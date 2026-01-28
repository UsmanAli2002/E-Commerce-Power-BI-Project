# E-Commerce-Power-BI- Dashboard-Project
o analyze sales data from an online e-commerce store and create an interactive Power BI dashboard highlighting key metrics, trends, and top-performing products and cities.

## Project Overview
This project analyzes sales data from an online e-commerce store and creates an **interactive Power BI dashboard**. The dashboard highlights key metrics, trends over time, top-performing products, and top-performing cities, allowing business stakeholders to make informed decisions.

---
## Dashboard


<img width="1318" height="752" alt="image" src="https://github.com/user-attachments/assets/9ce6b88f-1acc-4d90-8d8f-78fa3e8da2ea" />

## Dataset
- **Source:** My own Online E-Commerce Store Zamanestore.com
- **Columns used:**
  - `Order_ID`
  - `Order_Date` (date only)
  - `Product_Name`
  - `Order_Amount` / `Total`
  - `City`
  - `Payment_Method`

---

## Data Preparation & Cleaning
- Removed null orders
- Kept only relevant columns
- Converted date-time column to **date only**
- Checked and corrected data types (Date, Text, Number)
- Renamed columns for clarity


---

## Power Query Transformations
- Filtered unnecessary data
- Removed null values
- Ensured consistent data types
- Applied column renaming for readability

<img width="420" height="420" alt="image" src="https://github.com/user-attachments/assets/c8d9a55a-ec8d-426c-987b-bde1a33fcbea" />

---

## DAX Measures Created

| Measure | Purpose |
|---------|---------|
| **Total Orders** | Count of all orders |
| **Net Revenue** | Revenue per order minus fixed cost (e.g., `SUM(Order_Amount) - 800*COUNT(Order_ID)`) |
| **Average Order Amount** | Average revenue per order |
| **Monthly Revenue** | Month-to-date revenue calculation |
| **Orders by City** | Number of orders per city |
| **Top City by Orders** | City with the highest number of orders |
| **Top Sales Date** | Date with the highest sales |
| **Revenue for Selected Product** | Revenue for a specific product |
| **Top Products (Top N Filter)** | Show top 3–4 products by revenue in charts |

---

## Dashboard Visualizations

### KPI Cards
- Total Orders  
- Net Revenue  
- Average Order Amount  
- Success Rate (if applicable)

### Time-Based Analysis
- Line chart: Orders over time  
- Line chart: Revenue over time  

### Product & City Analysis
- Bar chart: Orders by City  
- Bar chart: Top 3–4 Products by Revenue  
- Card: Top City by Orders  
- Card: Top Sales Date  

### Detailed Table
- Columns: `Order_Date`, `Product_Name`, `Order_Amount`, `City`, `Payment_Method`, `Net Revenue`

### Interactive Slicers
- Date (Month/Year)
- City
- Product_Name

> All visuals are interactive — selecting values in slicers filters the charts and table dynamically.

---

## How to Explore
1. Open `Ecommerce_PowerBI_Dashboard.pbix` in **Power BI Desktop**.
2. Use slicers to filter data by:
   - Date (month/year)
   - City
   - Product
3. Hover over charts to view exact values.
4. Interact with the dashboard to analyze KPIs, trends, and top-performing entities.


