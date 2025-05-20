## **Netflix Dashboard Analysis**

This Power BI dashboard provides a comprehensive view of **Netflix's media performance and stock analysis** by combining content-level data with financial stock metrics. It is designed using **data modeling, DAX calculations**, and a visually compelling layout for storytelling and analytics.

---

### 📂 **File Format:**

* `.pbix` (Power BI Desktop file)

---

### 🔍 **Dashboard Sections:**

#### **1. Netflix Media Analysis (First Page)**

* **Slicer:** Year range filter (2009 to 2022)

* **Visuals:**

  * **Top Titles by Release Year**
  * **Content Type Runtime:** Comparison between Movies and Shows
  * **Gauge Chart:** Total Ratings (5335)
  * **Bar Chart:** Watching Time by Year (2013–2022)
  * **Top 6 Genres by Runtime**

* **Insights:**

  * Comedy has the highest runtime.
  * Peak watching time occurred in 2019 and 2020.
  * Content release is filtered dynamically across years.

---

#### **2. Netflix Stock Analysis (Second Page)**

* **Top/Bottom Dates with Highest and Lowest Stock Prices**

* **Line and Area Chart:** High vs. Low prices by date

* **Comparative Bar Charts:**

  * Lowest Stock Prices vs. Open Prices
  * Highest Stock Prices vs. Open Prices

* **Insights:**

  * Highest recorded stock price: \$700.99 on 17-11-2021
  * Lowest recorded stock price: \$236.11 on 09-02-2018
  * Stock data visualized by key dates with tooltip interactivity

---

### 🧮 **DAX Functions Used:**

* `CALCULATE()`, `SUM()`, `FILTER()`, `MAX()`, `MIN()`, `DATE()`
* Time intelligence: `YEAR()`, `DATESYTD()`, `TOTALYTD()`
* Conditional formatting logic using `SWITCH()` or `IF()` for color-coded indicators (high/low stock)

---

### 🧱 **Data Modeling:**

* **Star Schema:**

  * Fact tables: `StockPrices`, `ContentMetrics`
  * Dimension tables: `Date`, `Genre`, `Title`, `Type`
* **Relationships:** One-to-many between date and content/stock metrics for time-based analysis
* **Measures and Calculated Columns:** For runtime totals, genre counts, max/min stock valuetoggles

---

### 🎯 **Purpose of the Dashboard:**

* Provide **media performance analytics** (viewing trends, genres, runtime) for content planning
* Deliver **financial insights** using stock trends and price fluctuations for stakeholders
* Enable data-driven decision-making for both **content strategy and investment review**

ScreenShot / Demo
https://github.com/Mahendra7805/NetfilxDashboard/blob/main/Netflix%201.png
https://github.com/Mahendra7805/NetfilxDashboard/blob/main/Netflix%202.png
