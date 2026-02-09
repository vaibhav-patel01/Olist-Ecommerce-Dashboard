# Olist-Ecommerce-Dashboard
This is an Olist ecommers data analysis Project , Solves the real world Business Problems

# 🛒 Olist E-Commerce Analytics Dashboard

### 📊 Project Overview
This project is a comprehensive **Full-Stack Data Analytics** solution built to analyze the Brazilian E-Commerce dataset (Olist). The goal was to provide actionable insights into sales performance, customer behavior, product logistics, and seller quality.

The solution leverages **MS SQL Server** as the primary data warehouse, uses **Python** for complex data fetching and cleaning, and visualizes the final results in **Power BI**.

---

### 🛠️ Tech Stack & Workflow

* **Data Source:** Microsoft SQL Server (Raw Data)
* **ETL & Processing:** Python (Pandas, SQL Alchemy/PyODBC)
* **Visualization:** Microsoft Power BI
* **Data Modeling:** Star Schema

**Workflow:**
1.  **Data Fetching:** Python scripts connect directly to the **MS SQL Server** database to query raw transaction, customer, and product data.
2.  **Data Cleaning:** Used Python (Pandas) to handle missing values, correct data types, and merge tables, ensuring the data is analysis-ready before visualization.
3.  **Visualization:** The processed data is loaded into **Power BI** to create interactive dashboards and monitor KPIs.

---

### 📱 Dashboard Features & Views

The report is divided into 4 key analytical views:

#### 1. 📈 Performance & Overview
*High-level KPIs for executive monitoring.*
* **Key Metrics:** Total Sales (**$10.9M**), Total Orders (**76.53K**), Average Order Value ($142.6), and Average Delivery Time (14 Days).
* **Trend Analysis:** Monthly and yearly sales trends to identify seasonality.
* **Payment Analysis:** Breakdown of payment methods, highlighting **Credit Card (78.6%)** as the dominant mode.
* **Geospatial:** Performance by State (Top State: SP).

#### 2. 👥 Customers & Performance
*In-depth analysis of customer retention and value.*
* **Customer Lifecycle:** Active vs. Inactive customers, with a calculated **Churn Rate of ~88.77%**.
* **RFM Analysis:** Segmentation of customers into clusters like *Potential Loyalists*, *Lost*, and *Recent Customers*.
* **CLV (Customer Lifetime Value):** Average CLV tracked at **$142.58**.
* **Regional Density:** Heatmaps showing customer concentration in Sao Paulo (SP), Rio (RJ), and Minas Gerais (MG).

#### 3. 📦 Products & Relation
*Insights into inventory, freight, and product quality.*
* **Inventory Metrics:** Total Products (32.9K) with a split between New vs. Existing products.
* **Logistics:** Average Freight Value ($23.47) analyzed against product categories.
* **Content Correlation:** Analysis of how *Product Photo Quantity* and *Description Length* correlate with sales volume.
* **Pareto Analysis:** Identification of the "Most Sold Products" to optimize stock for high-demand items.

#### 4. ⭐ Sellers Performance & Reviews
*Monitoring vendor quality and operational efficiency.*
* **Seller KPIs:** Total Sellers (3K+), with **8.87%** Delay Percentage.
* **Rating Analysis:** Average Seller Rating (**4.09/5**). A Sankey-style breakdown connects Product Categories to Delivery Status and Review Scores.
* **Top Performers:** Leaderboard of top sellers by revenue and volume to identify key partners.

---

### 🧠 Key Analytical Insights
* **Geography is Key:** The state of **Sao Paulo (SP)** dominates both the seller base and customer base, suggesting logistics strategies should be centered there.
* **Churn is High:** With an 88% churn rate, the business relies heavily on new customer acquisition rather than retention. A loyalty program is recommended.
* **Review Correlation:** Products with "Early Delivery" status consistently correlate with higher "5-Star" ratings, validating that logistics speed is the primary driver of customer satisfaction.

---

### ⚙️ Setup Instructions

**Prerequisites:**
* Python 3.x (Libraries: `pandas`, `pyodbc` or `sqlalchemy`)
* Microsoft SQL Server (with Olist database restored)
* Power BI Desktop

**Steps:**
1.  **Database Connection:** Ensure your local MS SQL Server instance is running.
2.  **Run ETL Script:** Execute `data_fetch.py`. This script connects to SQL, cleans the data, and prepares it for the dashboard.
3.  **Load Dashboard:** Open `Olist_Dashboard.pbix` in Power BI.
4.  **Refresh Data:** Ensure the Python path is correctly set in Power BI options to allow the data refresh.

---

### 👤 Author

**Surendra Kumar**
*Full Stack Data Analyst*
* [LinkedIn Profile](#)
* [Portfolio Website](#)
