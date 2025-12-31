# 🎯 TechStyle Store Analytics Dashboard

This project demonstrates a **complete data analytics workflow** from **synthetic data generation** to **interactive visualization**, simulating a real-world e-commerce business scenario for **TechStyle Store**, an online retailer of:

* Electronics
* Home & Kitchen
* Clothing
* Sports & Outdoors
* Books & Stationery

---

## 💼 Business Problem

TechStyle Store management needs answers to critical questions:

* What is our **overall sales performance** and **profitability**?
* Which **product categories and items** are top performers?
* How are **customers segmented**, and what are their buying patterns?
* What is the **order fulfillment efficiency**?
* Which **geographic regions** generate the most revenue?
* Are there **seasonal trends** in sales?

> This dashboard provides actionable insights to support **data-driven decision-making** across **sales, marketing, and operations teams**.

---

## 🗃️ Dataset

### Data Generation

The dataset is **synthetically generated using Python**, with realistic business logic including:

* Seasonal sales patterns (holiday spikes in Nov-Dec) 🎄
* Customer registration timelines
* Realistic product pricing & cost structures 💰
* Multiple order statuses and payment methods
* Customer segmentation: **Regular, Premium, VIP**

### Database Schema

The project uses a **star schema**:

**Fact Table:**

* `order_details` - Transaction line items (~4,000+ records)

**Dimension Tables:**

* `customers` - Customer information (500 records)
* `products` - Product catalog (50 products across 5 categories)
* `orders` - Order header information (~2,000 orders)

---

### Data Dictionary

| Table         | Key Fields                                                                                  | Description                       |
| ------------- | ------------------------------------------------------------------------------------------- | --------------------------------- |
| customers     | customer_id, first_name, last_name, email, city, state, registration_date, customer_segment | Customer demographics and profile |
| products      | product_id, product_name, category, price, cost, stock_quantity                             | Product catalog with pricing      |
| orders        | order_id, customer_id, order_date, status, payment_method                                   | Order header information          |
| order_details | order_detail_id, order_id, product_id, quantity, unit_price, discount                       | Transaction line items            |

---

## ✨ Key Features

### 📊 Dashboard KPIs

* **Total Revenue** – Overall sales performance
* **Total Profit** – Net profitability
* **Profit Margin %** – Profitability efficiency
* **Total Orders** – Transaction volume
* **Average Order Value** – Customer spending behavior

### 📈 Visualizations

* **Revenue Trend Analysis** – Line chart showing sales over time
* **Category Performance** – Bar chart of revenue by product category
* **Order Status Distribution** – Pie chart of order fulfillment stages
* **Top Products** – Table showing best-selling items
* **Customer Segmentation** – Analysis by customer tier
* **Geographic Distribution** – Map visual of sales by state
* **Payment Method Analysis** – Breakdown of transaction types

### 🔄 Interactive Features

* Date range slicers for **time-period analysis**
* Category filters for **product analysis**
* Customer segment filters
* Cross-filtering across all visuals

---

## 🛠️ Technologies Used

* **Python 3.x** – Data generation

  * `pandas` – Data manipulation
  * `numpy` – Numerical operations
  * `datetime` – Date/time handling
* **Power BI Desktop** – Data visualization and dashboard creation

  * DAX – Calculated measures and columns
  * Power Query – Data transformation
* **Google Colab** – Cloud-based Python environment

---

## 🚀 How to Get Started

1. Clone this repository
2. Run the Python script to generate synthetic data
3. Import the dataset into Power BI Desktop
4. Explore KPIs and interactive dashboards
5. Filter by date, category, or customer segment to gain insights

---

