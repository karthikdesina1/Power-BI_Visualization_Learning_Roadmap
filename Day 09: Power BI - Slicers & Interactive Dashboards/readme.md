# Power BI: Slicers & Interactive Dashboards

A hands-on learning project covering **slicers** and **interactive dashboards** in Power BI: how to filter data visually and build reports users can explore without touching the underlying dataset.

![Power BI Slicers Infographic](powerbi_slicers_linkedin.png)

## Overview

Slicers are on-canvas visual filters. A user picks a value such as a date, region, category, product or customer, and every connected visual updates instantly. Combined with good layout, they turn a static report into an interactive dashboard.

## Topics Covered

- What slicers are and why they are used
- How slicers work inside dashboards
- Types of slicers
- Creating slicers step by step
- Connecting slicers to visuals
- Building interactive dashboards
- Real-time examples and hands-on practice

## Slicer Types

| Type | Best for |
|------|----------|
| **List** | Checkbox-style selection of a few values |
| **Dropdown** | Long lists where space is limited |
| **Between / Range** | Dates and numeric ranges |
| **Relative Date** | Rolling periods such as last 30 days |
| **Tile / Button** | Quick, button-style picks |

## How to Create a Slicer

1. Open your report in Power BI Desktop.
2. In the **Visualizations** pane, select **Slicer**.
3. Drag a field (e.g. `Region`, `Category`, `Order Date`) into the slicer's **Field** well.
4. In **Format**, choose the slicer style (List, Dropdown, Between, Tile) and adjust layout, colors and selection options.
5. Open **Format > Edit interactions** to control which visuals the slicer filters.
6. Click values in the slicer and confirm every connected visual updates.

## Connecting Slicers with Visuals

By default, a slicer filters every visual on the same page. To change this:

- Select the slicer, then go to **Format > Edit interactions**.
- On each visual, choose **Filter** (apply) or **None** (ignore).
- Use **Sync slicers** (View tab) to share one slicer across multiple pages.

## Building an Interactive Dashboard

Recommended layout:

- **Top:** KPI cards (Sales, Profit, Customers)
- **Left or top bar:** slicers (Date, Region, Category)
- **Center:** main charts (bar, line, map)
- **Bottom:** detail table or matrix

Tips:

- Keep slicers grouped and consistently placed.
- Limit each page to the slicers that matter.
- Use a clear **Clear selections** option (Ctrl + click to multi-select).
- Add bookmarks for common views.
- Test with different selections so no visual breaks or goes empty.

## Real-Time Examples

- Date-wise filtering
- Region-wise sales analysis
- Category-wise filtering
- Product performance dashboard
- Customer data analysis
- Sales and profit comparison
- Business performance tracking

## Repository Structure

```
.
├── README.md
├── powerbi_slicers_linkedin.png   # Infographic
├── data/                          # Sample dataset(s)
├── PowerBI/
│   └── slicers_dashboard.pbix     # Power BI report file
└── screenshots/                   # Dashboard screenshots
```

## Getting Started

**Requirements**

- Power BI Desktop (free, Windows)
- A sample dataset such as Superstore Sales (Excel or CSV)

**Steps**

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   ```
2. Open `PowerBI/slicers_dashboard.pbix` in Power BI Desktop.
3. If prompted, update the data source path under **Transform data > Data source settings**.
4. Click the slicers and explore how the visuals respond.

## Key Takeaways

- Slicers let users control what data they see.
- Filtering changes the view, never the underlying dataset.
- Good layout plus the right slicer type makes dashboards faster to use and easier to read.
- Edit interactions and sync slicers give you precise control over behavior.

## Resources

- [Power BI documentation: Slicers](https://learn.microsoft.com/power-bi/visuals/power-bi-visualization-slicers)
- [Power BI documentation: Edit interactions](https://learn.microsoft.com/power-bi/create-reports/service-reports-visual-interactions)
