# 📘 Dashboard Overview & Design Decisions

## Purpose
The goal of this dashboard is to provide a **clear executive overview** of sales performance while maintaining analytical depth for further exploration.

The focus is on:
- Clarity over visual clutter
- Business relevance over technical complexity
- Real-world data behavior rather than cleaned demo results

---

## Data Model
The dashboard uses a **star schema** consisting of:
- Fact table: Sales
- Dimension tables: Date, Product, Customer, Territory, Reseller

This structure ensures:
- Efficient filtering
- Clear relationships
- Scalable design for future enhancements

---

## KPI Design Rationale
| KPI | Business Purpose |
|----|------------------|
| Total Revenue | Overall sales performance |
| Total Profit | Business profitability |
| Profit Margin % | Quality of revenue |
| Total Orders | Customer demand |
| Total Quantity | Sales volume |

Profit and margin values are conditionally formatted to highlight loss-making scenarios.

---

## Handling Negative Values
Negative profit and margin values are intentionally preserved to:
- Reflect real operational losses
- Identify underperforming categories or channels
- Avoid misleading, overly-optimized reporting

This aligns with real-world business intelligence practices.

---

## Fiscal Year Handling
- Blank fiscal periods are excluded at the visual level to improve reporting clarity.
- FY2021 is excluded due to the absence of actual sales data.

No modifications were made to the raw dataset.

---

## Design Principles
- Consistent spacing and alignment
- Limited color palette
- Emphasis on KPIs and trends
- Minimal use of decorative elements

The dashboard is designed for fast interpretation by non-technical stakeholders.

---

## Future Improvements
- Drill-through pages for category-level deep dives
- Tooltips with additional contextual metrics
- Forecast vs actual comparison

---

## Author
Ahmed Tarek  
Data Scientist & Machine Learning Engineer
