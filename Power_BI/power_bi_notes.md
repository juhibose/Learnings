# 📊 Power BI – Consolidated Notes

Power BI is a **Microsoft business analytics tool** used to connect to various data sources, transform the data, and create interactive dashboards and reports for better decision-making.

---

## 1. What is Power BI?

Power BI is a **data visualization and business intelligence tool** that helps you:

- Connect to different data sources  
- Clean and transform data  
- Build dashboards and reports  
- Share insights across the organization  

**Example Use Case:**  
📌 An e-commerce company can use Power BI to track **sales trends**, **customer behavior**, and **profit margins** in real-time.

---

## 2. Power BI Components

| Component             | Description |
|----------------------|-------------|
| **Power BI Desktop**  | Windows application for building reports and dashboards. Includes **Power Query** for data transformation and **DAX** for calculations. |
| **Power BI Service**  | Online platform to publish, share, and collaborate on dashboards. |
| **Power BI Gateway**  | Connects on-premises data sources to Power BI Service for scheduled refreshes. |
| **Power BI Mobile**   | Mobile app to view dashboards and reports on the go. |
| **Power BI Report Builder** | Used to create paginated reports (print-friendly). |
| **Power BI Embedded** | Embed Power BI dashboards into custom applications. |

---

## 3. Power BI Workflow

1. **Connect** → Load data from Excel, CSV, SQL, APIs, etc.  
2. **Transform** → Use Power Query to clean, filter, merge, and shape data.  
3. **Model** → Build relationships between tables and optimize performance.  
4. **Visualize** → Create dashboards and reports with interactive visuals.  
5. **Publish** → Share reports using Power BI Service or embed into apps.

---

## 4. Key Concepts

### a. Power Query Editor (ETL Tool)
- Used for **data cleaning and transformation**.
- Actions you can perform:
  - Remove duplicates, blanks, and nulls  
  - Merge & append tables  
  - Pivot & unpivot data  
  - Change data types  

### b. Data Modeling
- Organize data into **tables and relationships**.
- **Star Schema** is preferred:
  - **Fact Table** → Contains transactional data (e.g., sales, revenue).  
  - **Dimension Tables** → Contains descriptive data (e.g., product, customer, region).  
- Types of connections:
  - **Import Mode** → Data is stored locally for faster performance.  
  - **DirectQuery Mode** → Data stays in the source for real-time analysis.

### c. DAX (Data Analysis Expressions)
DAX is a **formula language** for calculations and aggregations in Power BI.

**Types of DAX Expressions:**
1. **Calculated Columns** → Row-level calculations stored in the table  
2. **Measures** → Aggregations calculated on the fly  

**Common DAX Functions:**

| Function       | Purpose |
|----------------|---------|
| `SUM()`        | Adds up all values in a column |
| `CALCULATE()`  | Changes the filter context of a calculation |
| `FILTER()`     | Returns a filtered table |
| `IF()`         | Implements conditional logic |
| `RELATED()`    | Fetches data from a related table |
| `TOTALYTD()`   | Calculates Year-To-Date totals |

**Example DAX Measures:**
```DAX
Total Sales = SUM(Sales[Amount])
Profit % = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Revenue]), 0)


## 5. Reports vs Dashboards

| Feature           | Reports                  | Dashboards                  |
|------------------|--------------------------|-----------------------------|
| **Source**       | Single dataset           | Can combine multiple datasets |
| **Pages**        | Multi-page               | Single-page                 |
| **Interactivity**| Highly interactive       | Limited interactivity       |
| **Usage**        | For in-depth analysis    | For quick monitoring        |

---

## 6. Common Visualizations

- **Bar / Column Charts** → Compare categories  
- **Line Charts** → Show trends over time  
- **Pie / Donut Charts** → Show proportions  
- **Matrix / Table** → Detailed tabular data  
- **Slicers** → Add filters to reports  
- **KPI Cards & Gauge Visuals** → Highlight key metrics  
- **Maps** → Geographic analysis  

---

## 7. Performance Optimization Tips

- Use **Star Schema** for faster queries  
- Avoid importing unnecessary columns  
- Use **measures** instead of calculated columns when possible  
- Prefer **Import Mode** over DirectQuery for smaller datasets  
- Aggregate data before importing when possible  

---

## 8. Security Features

- **Row-Level Security (RLS)** → Restrict data visibility based on user roles  
- **Workspace Roles**:
  - **Viewer** → Can view dashboards only  
  - **Contributor** → Can edit reports  
  - **Member/Admin** → Full access  

---

## 9. Useful Resources

*(Add your favorite links, blogs, and tutorials here)*

