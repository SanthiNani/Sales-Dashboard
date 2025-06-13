# 📊 Simple Sales Dashboard Design using Power BI

## 🎯 Objective

The goal of this project is to design a clean, interactive sales dashboard using **Power BI**. The dashboard helps visualize sales performance across:
- Time (Month-Year)
- Region
- Product Category

This project is a basic introduction to building effective data visualizations for business intelligence, allowing stakeholders to easily understand and analyze trends.

---

## 📁 Dataset

**File Name:** `Superstore_Sales.csv`  
**Columns Included:**
- `Order Date`: The date when the order was placed.
- `Region`: The geographic area where the order was fulfilled (East, West, South, Central).
- `Category`: The product category (Technology, Furniture, Office Supplies).
- `Sales`: Revenue from the sale.
- `Profit`: Profit earned from the sale.

> ✅ **Note**: This dataset mimics the classic Superstore dataset used for dashboarding practice.

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Building interactive visualizations |
| *(Optional)* Python (Pandas) | Cleaning or preprocessing the dataset |

---

## 🧱 Steps Taken to Build the Dashboard

### 1. **Importing Data**
- Loaded `Superstore_Sales.csv` into Power BI using **Get Data > Text/CSV**.

### 2. **Date Formatting**
- Created a new column `MonthYear` to display order dates in `MMM YYYY` format.
- DAX Formula used:
  ```DAX
  MonthYear = FORMAT([Order Date], "MMM YYYY")
````

* Created another column to sort months correctly:

  ```DAX
  MonthNumber = MONTH([Order Date])
  ```
* Used **Sort by Column** to ensure chronological order in visuals.

### 3. **Creating Visuals**

#### 📈 Line Chart – Sales Over Time

* X-axis: `MonthYear`
* Y-axis: Sum of `Sales`
* Line color: **Teal Blue** (`#1F77B4`)

#### 📊 Bar Chart – Sales by Region

* Axis: `Region`
* Values: Sum of `Sales`
* Custom colors used for clarity:

  * West: `#4E79A7`
  * East: `#59A14F`
  * South: `#F28E2B`
  * Central: `#B07AA1`

#### 🍩 Donut Chart – Sales by Category

* Legend: `Category`
* Values: Sum of `Sales`
* Used contrasting colors for easy category comparison

### 4. **Adding Interactivity**

* Added **Slicer** for `Region` so users can filter views dynamically.
* Visuals are interconnected for cross-filtering.

### 5. **Highlighting Top Performers**

* Used **conditional formatting** in the bar chart to highlight the top region.
* Manually assigned color codes to emphasize high-sales categories and months.

---

## 📌 Key Insights

1. **West region** consistently outperformed all others, with peak sales during **Q2 and Q3**.
2. The **Technology category** generated the highest revenue across all regions.
3. **November** marked the highest monthly sales, likely due to seasonal shopping trends.

---

## 📤 Deliverables

| File Name              | Description                                                |
| ---------------------- | ---------------------------------------------------------- |
| `Sales_Dashboard.pbix` | Power BI project file containing the interactive dashboard |           |
| `Sales_Insights.txt`   | Plain text summary of top 3 business insights              |
| `README.md`            | Full project documentation (this file)                     |

---

## 🧠 Learning Outcome

By completing this task, you’ll gain hands-on experience in:

* Loading and transforming data in Power BI
* Creating meaningful visuals using real sales data
* Applying color theory to highlight trends and performance
* Summarizing data for business communication
  
---

## 👤 Author

**Santhi Raju Peddapati**
B.Tech in Computer Science (AI & ML)
Andhra Loyola Institute of Engineering & Technology
Email: [santhirajucs@gmail.com](mailto:santhirajucs@gmail.com)
GitHub: [github.com/santhirajucs](https://github.com/SanthiNani)

---

## 📌 Tags

`Power BI` `Dashboard` `Sales Analysis` `Superstore` `Business Intelligence` `Data Visualization`

```
