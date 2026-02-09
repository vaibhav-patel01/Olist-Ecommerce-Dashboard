# Olist-Ecommerce-Dashboard
This is an Olist ecommers data analysis Project , Solves the real world Business Problems

# 🛒 Olist E-Commerce Analytics Dashboard

### 📊 Project Overview
This project is a comprehensive **Full-Stack Data Analytics** solution built to analyze the Brazilian E-Commerce dataset (Olist). The goal was to provide actionable insights into sales performance, customer behavior, product logistics, and seller quality.

The solution leverages **MS SQL Server** as the primary data warehouse, uses **Python (via Jupyter Notebooks)** for complex data fetching and cleaning, and visualizes the final results in **Power BI**.

---

### 🛠️ Tech Stack & Workflow

* **Data Source:** Microsoft SQL Server (Raw Data)
* **ETL & Analysis:** Python (Pandas, PyODBC), Jupyter Notebook
* **Visualization:** Microsoft Power BI
* **Data Modeling:** Star Schema

**Workflow:**
1.  **Data Fetching:** Python code (executed in Jupyter) connects directly to the **MS SQL Server** database to query raw transaction, customer, and product data.
2.  **Data Cleaning & EDA:** Used **Jupyter Notebooks** to interactively clean the data (handling missing values, type casting) and perform initial Exploratory Data Analysis (EDA) to understand distributions and outliers.
3.  **Visualization:** The processed data is loaded into **Power BI** to create interactive dashboards and monitor KPIs.

---

### 📱 Dashboard Features & Views

The report is divided into 4 key analytical views. Below is a detailed breakdown of the visuals and insights from each page:

#### 1. 📈 Performance & Overview (Home Page)
*High-level executive summary of business health.*

* **Key Performance Indicators (KPIs):**
    * **Total Sales:** $10.9M
    * **Total Orders:** 76.53K
    * **Average Order Value (AOV):** $142.6
    * **Average Delivery Time:** 14 Days
    * **Total Quantity Sold:** 89K
    * **Order Status:** 625 Canceled, 301 Processing.
* **Visuals & Insights:**
    * **Trend by Months and Years (Line Chart):** visualizes the sales trajectory from 2016 to 2018, showing consistent growth with a significant peak in late 2017.
    * **Payment Method Contribution (Donut Chart):** Highlights **Credit Card** as the dominant payment method (78.6%), followed by Boleto (17.16%) and Voucher (3.04%).
    * **Product Categories Performance (Bar Chart):** A toggle-enabled chart showing Top 20 vs. Bottom 20 categories. "Bed Bath Table" and "Health Beauty" are leading categories.
    * **Sales Percentage Change (Area Chart):** Tracks the month-over-month variance in category performance.
    * **Performance by States (Bar Chart):** **SP (Sao Paulo)** is the top-performing state, significantly outperforming RJ (Rio) and MG (Minas Gerais).

#### 2. 👥 Customers & Performance
*In-depth analysis of customer retention, churn, and value.*

* **Key Performance Indicators (KPIs):**
    * **Total Active Customers:** 99.441K
    * **Inactive Customers (Last 12 Months):** 40K
    * **Repeated Customers:** 4.552K
    * **CLV Score:** $142.58
    * **Churn Rate:** 88.77%
    * **Avg Quantity Purchased:** 1.10
* **Visuals & Insights:**
    * **Churn Rate Over Time (Line Chart):** Tracks customer attrition, revealing a massive spike in Churn Rate around Jan 2017, stabilizing afterwards.
    * **Performance by RFM Segments (Bar Chart):** Segments customers based on Recency, Frequency, and Monetary value. The largest segment is **"Potential Loyalist" (6.3M)**, followed by "Lost" (4.4M).
    * **Customer Density by Region (Table):** Detailed breakdown showing Sao Paulo has the highest density (15,540 customers).
    * **Most Valuable Customers (Table):** Lists individual customer IDs ranked by Sales and Quantity to identify high-net-worth individuals.
    * **Most Liked Product (Table):** "Fashion Childrens Clothes" holds the highest average review score (5.00).

#### 3. 📦 Products & Relation
*Insights into inventory, freight costs, and content optimization.*

* **Key Performance Indicators (KPIs):**
    * **Total Products:** 32.951K
    * **Avg Freight Value:** $23.47
    * **Total New Products:** 10K
    * **Total Existing Products:** 23K
    * **Last 90 Days Sales:** 2.05M
* **Visuals & Insights:**
    * **New and Existing Products Performance (Table):** Compares sales between established and new inventory. "Watches Gifts" and "Health Beauty" have high counts of both.
    * **Relation Between Products Photo & Description Length (Line Chart):** Analyses if better product listings drive sales. Shows a correlation where optimal description length aligns with higher average quantities.
    * **Quality and Satisfaction Breakdown (Decomposition Tree):** A flow analysis starting from **Product Category -> Delivery Status -> Price Range -> Weight Range**. It highlights that "Bed Bath Table" has a significant number of "Early Deliveries" (562) compared to "Late".
    * **Most Sold Products (Table):** granular list of `product_id`s with the highest order counts.

#### 4. ⭐ Sellers Performance & Reviews
*Monitoring vendor quality and operational efficiency.*

* **Key Performance Indicators (KPIs):**
    * **Total Registered Sellers:** 3.095K (2.81K Active)
    * **Delay Percentage:** 8.87%
    * **Average Seller Rating:** 4.09 / 5
    * **Total Least vs. High Rated Sellers:** 396 vs. 2K
* **Visuals & Insights:**
    * **Sellers Count Over Time (Bar Chart):** Shows a steady increase in seller onboarding from 2016 to mid-2018.
    * **Rating Description and Performance (Table):** Shows **43,541 Excellent (5 Star)** reviews vs. 8,267 Garbage (1 Star) reviews, indicating generally high satisfaction.
    * **Region Contribution by Sellers (Table):** Sao Paulo (SP) contributes the most sellers (695), followed by Curitiba (PR) and Rio (RJ).
    * **Sellers Local Sales Percentage (Table):** Analyzes how much of a seller's volume is local vs. long-distance.

---

### ⚙️ Setup Instructions

**Prerequisites:**
* Python 3.x (Anaconda or standard install)
* Jupyter Notebook
* Microsoft SQL Server (with Olist database restored)
* Power BI Desktop

**Steps:**
1.  **Database Connection:** Ensure your local MS SQL Server instance is running and the Olist database is accessible.
2.  **Run Notebook:** Open the `data_cleaning.ipynb` file in Jupyter. Run the cells to fetch data from SQL, process it, and prepare the dataset.
3.  **Load Dashboard:** Open `Olist_Dashboard.pbix` in Power BI.
4.  **Refresh Data:** Ensure the Power BI data source settings point to the output of your Python logic or the SQL database directly.

---

### 👤 Author

**Vaibhav Patel**
*Full Stack Data Analyst*
* [https://www.linkedin.com/in/vaibhav-patel-5639aa355/](#)
* [Portfolio Website](#)
