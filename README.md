# 🍽️ Swiggy Sales Analysis | SQL End-to-End Case Study | EDA

## 📌 Project Overview

This project is a complete **end-to-end SQL-based data analysis case study** on Swiggy food delivery data. It focuses on transforming raw, unstructured data into a clean, optimized analytical model and extracting meaningful business insights.

The project covers:

* Data Cleaning & Validation
* Dimensional Modeling (Star Schema)
* KPI Development
* Exploratory Data Analysis (EDA)

---

## 🎯 Business Problem

Swiggy operates across multiple cities, restaurants, and cuisines. However, raw operational data often contains inconsistencies, duplicates, and lacks structure for analysis.

The objective is to:

* Ensure high-quality, reliable data
* Structure the dataset for efficient querying
* Analyze customer behavior, sales trends, and performance metrics
* Provide actionable business insights

---

## 🧹 Step 1: Data Cleaning & Validation

The raw dataset (`swiggy_data`) was processed to ensure accuracy and consistency.

### ✔️ Key Cleaning Steps:

* **Null Value Check** → Identified missing values across all critical columns
* **Blank Value Handling** → Removed empty string records
* **Duplicate Detection** → Grouped data using business-critical fields
* **Duplicate Removal** → Applied `ROW_NUMBER()` to retain only one valid record

👉 Result: Clean, reliable dataset ready for analysis

---

## 🏗️ Step 2: Data Modeling (Star Schema)

To improve performance and scalability, a **Star Schema** was implemented.

### 📊 Dimension Tables:

* `dim_date` → Date, Year, Month, Quarter, Week
* `dim_location` → State, City, Location
* `dim_restaurant` → Restaurant Name
* `dim_category` → Cuisine
* `dim_dish` → Dish Name

### 📌 Fact Table:

* `fact_swiggy_orders`

  * Price (INR)
  * Rating
  * Rating Count
  * Foreign Keys to all dimensions

👉 This structure reduces redundancy and enables fast analytical queries.

---

## 📊 Step 3: KPI Development

### 🔹 Core Business Metrics:

* Total Orders
* Total Revenue (INR Million)
* Average Dish Price
* Average Rating

These KPIs provide a quick snapshot of platform performance.

---

## 📈 Step 4: Exploratory Data Analysis (EDA)

### 📅 Time-Based Analysis

* Monthly Order Trends
* Quarterly Trends
* Year-wise Growth
* Day-of-Week Patterns

---

### 🌍 Location-Based Analysis

* Top 10 Cities by Order Volume
* Revenue Contribution by States

---

### 🍽️ Food Performance Analysis

* Top 10 Restaurants by Orders
* Top Categories (Cuisine-wise)
* Most Ordered Dishes
* Cuisine Performance (Orders + Avg Rating)

---

### 💰 Customer Spending Analysis

Orders were segmented into pricing buckets:

* Under ₹100
* ₹100–199
* ₹200–299
* ₹300–499
* ₹500+

👉 Used to understand customer purchasing behavior and pricing trends.

---

### ⭐ Ratings Analysis

* Distribution of ratings (1–5)
* Customer satisfaction insights

---

## 🧠 Key Insights

* Majority of orders fall within mid-range pricing (₹100–₹299)
* Certain cities contribute significantly higher order volumes
* High-demand dishes drive overall engagement
* Ratings indicate generally positive customer satisfaction
* Some categories show high demand but lower ratings (optimization opportunity)

---

## 🛠️ Tools & Technologies

* SQL (MySQL)
* Data Modeling (Star Schema)
* Exploratory Data Analysis

---

## 📂 Project Structure

swiggy-sql-eda-case-study/
│
├── data/
├── sql/
├── outputs/
├── images/
└── README.md

---

## 🚀 How to Use This Project

1. Load the raw dataset into MySQL
2. Run SQL scripts in sequence:

   * Data Cleaning
   * Dimension Table Creation
   * Fact Table Creation
   * Data Loading
   * KPI & Analysis Queries
3. Explore insights using SQL queries

---

## 💡 What I Learned

* Real-world data cleaning challenges
* Importance of structured data modeling
* Writing efficient analytical SQL queries
* Translating raw data into business insights

---

## 📌 Conclusion

This project demonstrates a complete SQL workflow from raw data to actionable insights.
It highlights how structured data modeling and analytical thinking can drive business decisions in real-world scenarios.

---

