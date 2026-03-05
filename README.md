# E-Commerce Sales Data Analysis – Excel

A comprehensive analysis of e-commerce sales performance across products, customers, regions, and time periods to identify revenue trends and customer purchasing behavior.

## 📖 Table of Contents

* [Project Overview](#-project-overview)
* [Data Source](#-data-source)
* [Tools & Technologies](#-tools--technologies)
* [Data Cleaning & Preparation](#-data-cleaning--preparation)
* [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
* [Key Insights](#-key-insights)
* [Recommendations](#-recommendations)
* [How to Use](#-how-to-use)

## 📊 Project Overview

This project focuses on analyzing **e-commerce sales data** to understand business trends, sales performance, and customer behavior.

The primary objectives were:

* To identify **top-selling product categories based on revenue**
* To analyze **month-wise sales performance**
* To evaluate **region-wise sales distribution**
* To understand **customer demographics and purchasing behavior**

The analysis was performed using **Microsoft Excel** by applying data cleaning techniques, calculated columns, pivot tables, and charts to generate meaningful business insights.

## 🗂️ Data Source

* Source: Simulated E-commerce Sales Dataset
* Format: Excel (.xlsx)
* Time Period: **2023 – 2025**

The dataset follows a **Fact-Dimension structure**.

**Tables in Dataset:**

* **Sales_Fact** – Transaction-level sales data
* **Customer_Dim** – Customer demographic details
* **Product_Dim** – Product information
* **Store_Dim** – Store and regional information

### Key Variables

**Customer_Dim**

* customer_id
* name
* age
* gender
* city
* state
* country

**Product_Dim**

* product_id
* product_name
* category
* sub_category
* brand
* cost
* stock

**Store_Dim**

* store_id
* store_name
* region
* city
* store_type

**Sales_Fact**

* sales_id
* order_date
* quantity
* unit_price
* discount
* payment_type
* total_amount

## 🛠️ Tools & Technologies

* **Data Analysis Tool:** Microsoft Excel
* **Data Cleaning and Transformation:** Excel Functions
* **Data Modeling Concept:** Fact-Dimension (Star Schema) Structure
* **Analysis Method:** Pivot Tables
* **Visualization:** Excel Charts

## 🧹 Data Cleaning & Preparation

Several preprocessing steps were applied to ensure data quality:

1. Handled **missing and inconsistent values** in both fact and dimension tables.
2. Standardized **data formats and column data types**.
3. Used **Find & Replace** to correct inconsistent values in fields such as Customer_ID and Country.
4. Created an **Age Group column** in the Customer_Dim table using conditional logic.
5. Calculated missing values for **Quantity, Discount, Unit Price, and Total Amount** in the Sales_Fact table using logical functions.
6. Estimated missing **Cost and Stock values** in Product_Dim using average-based imputation.

**Example Formula Used**

Age Group Classification:

```excel
=IF([@Age]<=30,"Youngsters",IF([@Age]<=50,"Middle-Age","Senior Citizen"))
```

These steps helped create a **clean, structured dataset ready for analysis**.

## 🔍 Exploratory Data Analysis (EDA)

The following business questions were explored:

* Which **product categories generate the highest revenue**?
* How does **sales performance vary month-wise**?
* Which **regions contribute the most to total sales**?
* How do **customer demographics influence sales**?

Visualizations created:

* Column Charts(Category-wise Revenue,Month-wise Sales,Customer demographics)
* Pie Chart(Store Region-wise Sales Distribution)
* Bar Chart(Top 5 product analysis)

## 💡 Key Insights

* **Home category** was the top revenue generator in **2023**, **Sports in 2024**, and **Electronics in 2025**.
* **Beauty and Clothing categories** showed relatively lower revenue compared to other product categories.
* In **2023 and 2024**, the **North region recorded the highest sales**, while the **East region performed better in 2025**.
* The **highest sales volume occurred in March, May, and July 2025**, exceeding 95 units.
* Sales showed **steady growth from early 2024 to mid-2025**, followed by a **sharp decline in October 2025**.
* **Female customers contributed more to total sales across all age groups** compared to male customers.
* Historical trends suggest **higher sales during festive seasons**.

## 🚀 Recommendations

* Offer **targeted discounts for slow-moving products** to improve sales performance.
* Strengthen **marketing campaigns during low-performing months** such as October and May.
* Prioritize **inventory planning for top-selling categories** to avoid stock shortages.
* Focus marketing efforts on **high-performing regions and customer segments**.
* Monitor seasonal trends to optimize **promotions during festive periods**.

## ⚙️ How to Use

To explore this project:

1. Download the **Excel dataset** from this repository.
2. Open the file using **Microsoft Excel**.
3. Navigate through the **analysis sheets and pivot tables**.
4. Use filters to explore:
   * Category performance
   * Region-wise sales
   * Month-wise trends
   * Customer demographics
5. Review charts and pivot tables to understand key insights.

No additional tools are required beyond **Microsoft Excel**.
