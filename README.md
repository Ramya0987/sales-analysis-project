# sales-analysis-project
# 🛒 Retail Sales Analysis

## 📌 Project Overview
This project analyzes **retail sales trends, customer behavior, and revenue insights** using SQL, Python, and data visualization.  
It covers **exploratory data analysis (EDA), SQL queries, business insights, and recommendations** for optimizing sales.

## 📊 Dataset
- **Synthetic dataset** with `1000`+ transactions
- Contains details on products, categories, prices, revenue, customer locations, and order dates.

## 📂 Project Structure
```
Retail_Sales_Analysis/
│── data/                   # (Optional: Dataset storage)
│── sales_analysis_sql.py    # SQL + Python script
│── sales_analysis.ipynb     # Jupyter Notebook with EDA & Visualizations
│── README.md                # Project documentation
│── images/                  # (Optional: Saved charts/graphs)
```

## ⚙️ Tools & Technologies
- **Python** (Pandas, Matplotlib, Seaborn, SQLite)
- **SQL** (SQLite for queries)
- **Jupyter Notebook** (for analysis)
- **Power BI (for visualizations)

## 📈 Key Insights
✔️ **Top-Selling Products & Categories**  
✔️ **Best-Performing Locations**  
✔️ **Seasonal Sales Trends**  
✔️ **Customer Spending Behavior (AOV Analysis)**  

## 📌 SQL Queries Used
```sql
-- Top 5 Best-Selling Products
SELECT product_name, SUM(total_revenue) AS total_sales
FROM sales_data
GROUP BY product_name
ORDER BY total_sales DESC
LIMIT 5;
```
```sql
-- Monthly Sales Trend
SELECT strftime('%Y-%m', order_date) AS month_year, SUM(total_revenue) AS total_sales
FROM sales_data
GROUP BY month_year
ORDER BY month_year;
```

## 📊 Visualizations
- Sales trends over time 📉
- Category-wise sales 📊
- Customer spending behavior 💰

## 🔥 Business Recommendations
- **Stock high-demand products** and optimize pricing strategies.
- **Expand in high-revenue locations** and introduce localized marketing.
- **Use seasonal trends** to plan discounts & marketing campaigns.

## 🚀 Next Steps
- Integrate **Power BI/Tableau Dashboard** 📊
- Automate **Monthly Sales Reports** using Python 📑

## ⭐ How to Run
1. Install **Python & Jupyter Notebook**.
2. Clone this repository manually or download the files.
3. Run `sales_analysis_sql.py` to execute SQL queries.
4. Open `sales_analysis.ipynb` to explore visualizations.

