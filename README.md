# ✈️ SQL Project – AirlineDB (PostgreSQL)

End-to-end SQL analysis project using PostgreSQL to extract operational and performance insights from a relational airline database.

---

## 📌 Project Overview

This capstone project focuses on querying and analyzing structured airline data using PostgreSQL.

The objective was to apply advanced SQL concepts to:

- Validate data integrity
- Standardize reporting formats
- Perform ranking and aggregation analysis
- Extract operational insights
- Support performance evaluation across multiple dimensions

**Database:** AirlineDB  
**SQL Engine:** PostgreSQL  

---

## 🧮 Analytical Tasks & Solutions

### 1️⃣ Data Integrity Validation  
**Problem:** Identify tickets without boarding passes.

**Approach:**
- Used `LEFT JOIN`
- Applied NULL filtering to detect missing relational records

**Outcome:**
- Identified 251 tickets without boarding passes

**Concepts Used:**
- JOIN operations  
- NULL handling  
- Data consistency validation  

---

### 2️⃣ Date Standardization  
**Problem:** Format booking dates into `YYYY-MM-DD`.

**Approach:**
- Used `TO_CHAR()` function for formatting

**Concepts Used:**
- Date formatting  
- Column transformation  

---

### 3️⃣ Product Demand Analysis (Store-Level Ranking)

**Problem:** Identify the most popular product in each store based on quantity sold.

**Approach:**
- Aggregated quantities using `SUM()`
- Applied `RANK()` window function
- Partitioned results by store

**Concepts Used:**
- CTE (Common Table Expressions)
- GROUP BY
- Window Functions
- Ranking Logic

---

### 4️⃣ Quarterly Sales Performance Comparison

**Problem:** Compare quarterly sales across stores and rank them.

**Approach:**
- Converted order dates to `YYYY-Q` format
- Calculated total sales using:
  
  `quantity * list_price * (1 - discount)`

- Applied window ranking per quarter

**Concepts Used:**
- Revenue computation logic
- Aggregation
- Partitioned ranking
- Time-based grouping

This analysis evaluates store-level performance across quarters and highlights competitive positioning.

---

### 5️⃣ Airport Traffic Concentration

**Problem:** Rank airports based on total departing flights.

**Approach:**
- Aggregated flights by departure airport
- Applied global ranking using `RANK()`

**Concepts Used:**
- Aggregation
- COUNT()
- Ranking functions
- Traffic concentration analysis

---

## 📊 Key Insights

- Identified data inconsistencies (tickets without boarding passes)
- Standardized reporting formats for consistent analysis
- Ranked store performance quarterly
- Determined product demand concentration per store
- Identified high-traffic airports based on departure volume

---

## 🛠 Skills Demonstrated

- PostgreSQL
- Complex JOINs
- CTE (WITH statements)
- Window Functions (RANK)
- Aggregation & Grouping
- Revenue Calculation Logic
- Time-based Analysis
- Relational Data Modeling
- Operational Insight Extraction

---

## 🎯 Conclusion

This capstone demonstrates structured SQL application for real-world operational analysis.

The project reflects the ability to:

- Validate relational integrity
- Perform advanced aggregations
- Apply ranking logic for performance comparison
- Extract decision-oriented insights from structured databases

It highlights practical SQL proficiency in analytical querying, business logic implementation, and relational data analysis.
