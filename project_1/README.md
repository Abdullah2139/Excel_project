# Customer Demographics & Sales Data Cleaning Project

## 📌 Project Overview
This project focuses on **cleaning and preparing** a dataset containing customer demographic details and sales transactions for further analysis.  
The dataset combines **customer information** (names, contact details, addresses, demographics) with **purchase data** (order details, product categories, and transaction values).

---

## 🗂 Dataset Details
- **File Name:** `Customer_demographics_and_sales.xlsx`
- **Total Rows:** 194
- **Total Columns:** 59
- **Sheet Name:** `Sheet1`
- **Key Categories:**
  - **Customer Information:** Name, gender, address, email, phone number, nationality, age, etc.
  - **Order Information:** Order ID, order date, shipping date, sales representative, order value, etc.
  - **Product Categories:** Baby products, beverages, snacks, household items, personal care, etc.

---

## 🧹 Data Cleaning Steps
During the cleaning process, the following operations were performed:

1. **Removed Duplicate Records**  
   - Identified and removed rows with repeated customer and order details.

2. **Handled Missing Values**  
   - Filled missing demographic fields (e.g., `STATE`, `EMAIL_ADDRESS`) using available reference data.
   - For numerical columns like `ORDER_VALUE`, imputed missing values with the median.

3. **Standardized Formats**  
   - Converted dates (`ORDER_DATE`, `ORDER_SHIP_DATE`) into a consistent format (`YYYY-MM-DD`).
   - Unified text casing for columns such as `CITY` and `STATE`.
   - Standardized phone numbers into a uniform format.

4. **Validated Data Consistency**  
   - Ensured `ORDER_SHIP_DATE` ≥ `ORDER_DATE`.
   - Checked that `AGE` values were within realistic bounds.

5. **Removed Irrelevant Columns**  
   - Dropped extra or redundant fields such as repeated name columns (`Customer_name` vs. `CUST_NAME`).

---

## 📊 Potential Analysis After Cleaning
- **Customer Segmentation** based on demographics and purchase history.
- **Sales Trends Analysis** by date, region, and product category.
- **Top Products** purchased by different customer segments.
- **Performance Tracking** of sales representatives.

---

## 🛠 Tools & Technologies
- **Excel** for initial inspection and cleaning.
- **Python (pandas)** for advanced cleaning, validation, and formatting.

---

## ✅ Outcome
The cleaned dataset is now:
- **Free of duplicates**
- **Consistently formatted**
- **Ready for analysis** in BI tools, Python, or statistical models.

---