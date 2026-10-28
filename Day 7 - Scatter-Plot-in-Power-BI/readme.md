# 📊 Scatter Plot in Power BI

## 📌 Overview

A **Scatter Plot** in Microsoft Power BI visualizes the relationship between two numerical variables.

Each point represents an observation, making it easier to explore **correlations, patterns, clusters, trends, and outliers**.

Scatter Plots are useful in business analytics, marketing, finance, customer analysis, education, and performance reporting.

---

## 🎯 1. What is a Scatter Plot?

A Scatter Plot displays observations using two numerical axes:

- **X-Axis:** First numerical variable
- **Y-Axis:** Second numerical variable

Example:

`X-Axis: Sales | Y-Axis: Profit`

Each point represents a product, customer, transaction, or other observation.

---

## 🔍 2. Why Use Scatter Plots?

Scatter Plots help analysts:

- Understand relationships between variables
- Identify positive and negative correlations
- Discover clusters and trends
- Detect outliers
- Compare performance across categories
- Investigate business opportunities and risks

---

## ⚙️ 3. Scatter Plot Fields in Power BI

| Field | Purpose | Example |
|---|---|---|
| X-Axis | First numeric measure | Sales |
| Y-Axis | Second numeric measure | Profit |
| Values/Details | Identifies observations | Product ID |
| Legend | Groups points by category | Product Category |
| Size | Controls bubble size | Quantity Sold |
| Tooltips | Additional information | Revenue, Margin |
| Play Axis | Animates data over time, where available | Year |

*Note: Field-well names and available features may vary by Power BI version.*

---

## 📈 4. Understanding Correlation

### Positive Correlation ↗️

Both variables tend to increase together.

**Example:** Marketing Spend vs. Revenue.

### Negative Correlation ↘️

As one variable increases, the other tends to decrease.

**Example:** Product Price vs. Units Sold.

### No Clear Correlation

No obvious linear relationship is visible.

**Example:** Two unrelated business metrics.

### Clusters

Groups of observations sharing similar characteristics.

**Example:** Customers with similar spending patterns.

### Outliers

Observations that differ significantly from the general pattern.

**Example:** A product with high sales but unusually low profit.

**Important:** Correlation does not establish causation.

---

## 🛠️ 5. Creating a Scatter Plot in Power BI

1. Open Power BI Desktop.
2. Import a dataset.
3. Select the **Scatter Chart** visual.
4. Add a numerical measure to the X-axis.
5. Add another numerical measure to the Y-axis.
6. Add an observation identifier to Values/Details to display separate points.
7. Add a category to Legend.
8. Optionally add Size and Tooltips.
9. Customize titles, colors, markers, and axis formatting.
10. Analyze relationships, clusters, and outliers.

---

## 💼 6. Real-World Applications

| Scenario | X-Axis | Y-Axis | Analytical Goal |
|---|---|---|---|
| Sales vs. Profit | Sales | Profit | Profitability patterns |
| Marketing vs. Revenue | Marketing Spend | Revenue | Marketing performance |
| Study Hours vs. Marks | Study Hours | Marks | Academic performance |
| Product Price vs. Sales | Price | Units Sold | Pricing relationships |
| Customer Analysis | Age | Spending | Customer behavior |
| Website Analytics | Traffic | Conversions | Conversion patterns |

---

## 🧮 7. Useful DAX Measures

**Total Sales**

```dax
Total Sales =
SUM(Sales[SalesAmount])
```

**Total Profit**

```dax
Total Profit =
SUM(Sales[Profit])
```

**Profit Margin %**

```dax
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
) * 100
```

**Total Quantity**

```dax
Total Quantity =
SUM(Sales[Quantity])
```

*Adjust table and column names to match your dataset.*

---

## 📊 8. Hands-On Example: Sales vs. Profit

### Objective

Analyze the relationship between product sales and profitability.

### Configuration

- **X-Axis:** Total Sales
- **Y-Axis:** Total Profit
- **Values/Details:** Product ID
- **Legend:** Product Category
- **Size:** Total Quantity
- **Tooltips:** Profit Margin %

### Questions to Investigate

- Do higher sales generally correspond to higher profits?
- Which products have high sales but low profits?
- Are there clusters of similarly performing products?
- Which observations are unusual?
- Do different product categories show different patterns?

### Expected Outcome

Identify profitability patterns, unusual products, and opportunities for further investigation.

---

## 📍 9. Scatter Plot vs. Line Chart

| Feature | Scatter Plot | Line Chart |
|---|---|---|
| Main purpose | Relationships | Trends |
| Typical X-axis | Numeric variable | Time/ordered category |
| Typical Y-axis | Numeric measure | Numeric measure |
| Best for | Correlation, clusters, outliers | Growth, decline, seasonality |

---

## 🎯 10. Key Takeaways

- Scatter Plots compare two numerical variables.
- Each point represents an observation.
- Colors distinguish categories.
- Bubble size can encode a third measure.
- Correlations reveal associations, not necessarily causes.
- Outliers may highlight risks or opportunities.
- Proper observation-level grouping is essential for meaningful analysis.

### Analytical Workflow

**Data → Relationships → Patterns → Clusters → Outliers → Insights → Decisions**

---

## 🧰 Tools & Concepts

- Microsoft Power BI
- Scatter Plot
- DAX Measures
- Correlation Analysis
- Outlier Detection
- Cluster Analysis
- Bubble Charts
- Business Intelligence
- Data Visualization
- Exploratory Data Analysis

