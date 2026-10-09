# Stylo Pakistan | Retail Operations & Profitability Intelligence

### 286M in Reported Sales. 60 Stores. One Retail Performance Story.

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black) ![DAX](https://img.shields.io/badge/DAX-Measures-blue) ![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green) ![Retail Analytics](https://img.shields.io/badge/Domain-Retail-purple)

**Power BI | Power Query | DAX | Star Schema | Retail Analytics**

<img width="1672" height="941" alt="Stylo retail operations dashboard overview" src="https://github.com/user-attachments/assets/7b513da5-1efa-402b-8328-20fa258aee20" />

> **Portfolio context:** An independent project using a **simulated dataset inspired by Stylo Pakistan**. Results below are dashboard-reported figures for the simulation, not verified Stylo company performance or evidence of an employer engagement.

---

## Executive Overview

**Strong sales are only the beginning of a useful retail story.** Management also needs to understand *where* revenue originates, *which* products contribute, *how* stores perform, and *whether* returns or channel concentration deserve attention.

I developed a three-page Power BI retail operations dashboard to bring sales, profit, stores, products, channels, and customer-related indicators into one interactive reporting experience. The project uses Power Query, a star-schema model, and DAX measures to translate transaction-level records into practical management questions.

**Central question:** *How can retail leaders move beyond headline sales and identify the stores, product groups, and channels that merit closer attention?*

---

## Executive KPI Snapshot

| KPI | Dashboard-reported value | What it helps assess |
|---|---:|---|
| Total Sales | **286M** | Overall sales scale |
| Total Profit | **132.93M** | Profit contribution |
| Profit Margin | **47%** | Profitability relative to sales |
| Total Orders | **26K** | Order activity |
| Average Order Value | **10.98K** | Sales per order |
| Return Rate | **7%** | Reported return exposure |
| Total Stores | **60** | Store footprint |
| Average Customer Rating | **4.05** | Recorded customer ratings |

*Values and units are presented as reported in the supplied project description; underlying data has not been independently audited here.*

---

## 01 | The Business Challenge

### Many Transactions. One Need for Clarity.

A multi-store retailer has to evaluate performance across cities, provinces, store types, product categories, and sales channels. Disconnected transaction reports make it harder to distinguish a high-sales category from a truly profitable one, or a leading store from one that is underperforming relative to its peers.

This case study explores four management questions:

1. **Growth:** Which stores, cities, and categories contribute most to sales?
2. **Profitability:** How do profit and margin vary across products and stores?
3. **Channel mix:** How dependent is the simulated business on physical stores versus online orders?
4. **Experience and returns:** Which customer-rating and return indicators warrant follow-up?

**Objective:** Create an interactive, cross-filtered performance view that supports more focused retail decisions.

---

## 02 | How I Approached the Analysis

### From Transaction Records to Decision-Ready Views

**Step 1 — Prepare the data.** Used **Power Query** to support the ETL workflow for the retail dataset.

**Step 2 — Model the business.** Organized the reporting model as a **star schema** with one sales fact table and seven related dimensions:

| Fact table | Dimension tables |
|---|---|
| `FactSales` | `DimDate`, `DimStore`, `DimProduct`, `DimCustomer`, `DimEmployee`, `DimPromotion`, `DimPaymentMethod` |

**Step 3 — Define consistent measures.** Created DAX calculations for sales, profit, order volume, order value, margin, returns, store averages, and product averages.

**Step 4 — Communicate the findings.** Structured three interactive reporting pages around the decisions of executives, store managers, and merchandising teams.

<img width="1622" height="969" alt="Stylo retail analytics star schema data model" src="https://github.com/user-attachments/assets/de8adaea-b40c-474a-a65a-375ea068cf58" />

---

## 03 | Dashboard Story: Three Views, Three Decisions

### Page 1 — Executive Overview: Where Is Retail Performance Coming From?

<img width="1153" height="675" alt="Stylo Power BI executive overview" src="https://github.com/user-attachments/assets/d3beac89-e602-49ed-8ff2-953209b92c9b" />

| KPI | Reported value |
|---|---:|
| Total Sales | **286M** |
| Total Profit | **132.93M** |
| Profit Margin | **47%** |
| Total Orders | **26K** |
| Average Order Value | **10.98K** |
| Return Rate | **7%** |

**What the dashboard shows:** Monthly sales trends, sales by product category, city, and order channel.

**Insight — Sales rely heavily on physical stores.** Store purchases account for approximately **80%** of reported revenue, compared with **20%** online. **Women's Shoes** is the leading sales category, and major cities contribute a substantial share of the business.

**Why it matters:** A store-heavy channel mix makes physical location performance central to revenue monitoring. Online sales represent a smaller but identifiable channel to evaluate on its own merits.

**Suggested action:** Compare channel profitability, sales trends, and customer behavior before deciding where to prioritize commercial investment.

### Page 2 — Store Performance: Are All Locations Contributing Equally?

<img width="1136" height="629" alt="Stylo Power BI store performance dashboard" src="https://github.com/user-attachments/assets/eccd87af-cb0a-4cb7-a625-a04d8a1c27cd" />

| KPI | Reported value |
|---|---:|
| Total Stores | **60** |
| Average Sales per Store | **4.76M** |
| Average Profit per Store | **2.22M** |
| Average Rating | **4.05** |
| Total Customers | **5K** |
| Return Rate | **7%** |

**What the dashboard shows:** Store-level performance matrix, top 10 stores, provincial sales, and city comparisons.

**Insight — Regional and store-level performance is uneven.** **Punjab** is the leading province by reported sales. Top-performing stores exceed **7M** in sales, while average recorded customer ratings are above **4.0**.

**Why it matters:** Regional leaders and store averages can be useful benchmarks, but high sales alone do not establish superior efficiency or profitability.

**Suggested action:** Compare stores using sales, profit, return rate, rating, and store type together; investigate the reasons behind meaningful outliers.

### Page 3 — Product Performance: Which Products Deserve More Attention?

<img width="1159" height="995" alt="Stylo Power BI product performance dashboard" src="https://github.com/user-attachments/assets/fc13e71c-8a95-49b2-b6e7-a12625b5c9dc" />

| KPI | Reported value |
|---|---:|
| Total Products | **250** |
| Total Categories | **7** |
| Average Product Sales | **1.14M** |
| Average Product Profit | **531.73K** |
| Average Selling Price | **4.97K** |
| Return Rate | **7%** |

**What the dashboard shows:** Leading products, category sales and profit, material contribution, gender-segment sales, and a detailed product table.

**Insight — Category and assortment mix shape sales.** **Women's Shoes** leads category sales; **Silk** leads the reported material contribution; products classified as **Female** represent approximately **75%** of sales.

**Why it matters:** Revenue contribution reveals where demand is concentrated but should be interpreted alongside margin and returns before making assortment decisions.

**Suggested action:** Evaluate high-revenue product segments against profitability and return behavior to identify potential merchandising priorities.

---

## 04 | From Findings to Management Questions

| Priority | Signal from dashboard | Management question | Proposed next step |
|---|---|---|---|
| High | ~80% of sales through stores | Are locations equally productive and profitable? | Compare store-level sales, profit, and returns |
| High | Women's Shoes leads sales | Does the largest category also lead profit? | Review category margins and product contributions |
| Medium | Punjab leads provincial sales | Which markets are over- or underperforming relative to their footprint? | Compare cities and stores with appropriate baselines |
| Medium | 7% reported return rate | Where are returns concentrated? | Segment returns by product, store, and channel |
| Medium | Average rating of 4.05 | Are weaker ratings associated with any specific segments? | Analyze rating distributions, not just averages |

*These are analytical follow-ups and recommendations, not claimed implemented improvements.*

---

## 05 | Core DAX Measures

The following expressions are preserved from the supplied project documentation.

### Sales, Profit, and Orders

```DAX
Total Sales =
SUM(FactSales[NetSales])

Total Profit =
SUM(FactSales[Profit])

Total Orders =
DISTINCTCOUNT(FactSales[InvoiceID])

Total Quantity =
SUM(FactSales[Quantity])

Average Order Value =
DIVIDE(
    [Total Sales],
    [Total Orders]
)

Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales]
)
```

### Returns

```DAX
Return Orders =
CALCULATE(
    COUNTROWS(FactSales),
    FactSales[Returned] = "Yes"
)

Return Rate % =
DIVIDE(
    [Return Orders],
    [Total Orders]
)
```

> **Measure-definition check:** `Return Orders` counts rows marked returned while `Total Orders` counts distinct invoices. If invoices can contain multiple rows, the resulting rate may not represent the share of distinct orders returned. Validate the dataset grain and intended denominator before treating 7% as an order-level return rate.

### Stores and Customer Experience

```DAX
Total Stores =
DISTINCTCOUNT(DimStore[StoreID])

Avg Store Sales =
DIVIDE(
    [Total Sales],
    [Total Stores]
)

Avg Profit Store =
DIVIDE(
    [Total Profit],
    [Total Stores]
)

Average Rating =
AVERAGE(FactSales[Rating])

Total Customers =
DISTINCTCOUNT(FactSales[CustomerID])
```

### Product Performance

```DAX
Total Products =
DISTINCTCOUNT(DimProduct[ProductID])

Total Categories =
DISTINCTCOUNT(DimProduct[Category])

Avg Product Sales =
DIVIDE(
    [Total Sales],
    [Total Products]
)

Avg Product Profit =
DIVIDE(
    [Total Profit],
    [Total Products]
)

Average Selling Price =
AVERAGE(FactSales[UnitPrice])
```

---

## 06 | Interactive Analysis

The report supports cross-filtering across **Year, Month, Province, Store Type, Category, Material, Membership Type, Order Channel, and Store Name**. These controls allow users to move from overall performance to more specific operational comparisons.

---

## 07 | Skills Demonstrated

- **Power BI:** Three-page dashboard design, KPI reporting, interactive filtering
- **Power Query:** Data preparation and ETL workflow
- **DAX:** Measures for revenue, profit, orders, averages, margins, and returns
- **Data Modeling:** Star schema using `FactSales` and seven dimensions
- **Retail Analysis:** Channel mix, store performance, regional comparisons, merchandising insights
- **Data Storytelling:** Translating dashboard results into management questions and proposed actions

---

## 08 | Repository Structure (Documented Layout)

The supplied project description lists the following intended repository organization. Confirm paths against the actual GitHub repository before using them as download links.

```text
Stylo-Retail-Operations-Dashboard/
├── Dashboard/
│   └── Stylo Retail Operations Dashboard.pbix
├── Dataset/
│   ├── FactSales.csv
│   ├── DimProduct.csv
│   ├── DimStore.csv
│   ├── DimCustomer.csv
│   ├── DimDate.csv
│   ├── DimEmployee.csv
│   ├── DimPromotion.csv
│   └── DimPaymentMethod.csv
├── Images/
│   ├── Executive Overview.png
│   ├── Store Performance.png
│   └── Product Performance.png
└── README.md
```

**Availability note:** A listed file path in this documentation does not by itself confirm the file is uploaded. The linked screenshots above are the supplied image assets.

---

## 09 | Future Enhancements

- Customer insights and cohort analysis
- Inventory availability and stock planning
- Forecasting, after validating appropriate historical data
- MTD, QTD, and YTD time-intelligence measures
- Drill-through analysis by store and product
- Power BI Service publication, where appropriate
- Row-level security for role-based reporting
- Validation of measures and reconciliation with the source dataset

---

## Final Business Takeaway

### Sales Show the Scale. Store, Product, and Channel Analysis Explain the Mix.

The Stylo retail simulation demonstrates how a structured Power BI model can turn transaction records into a cohesive performance story: **what sells, where revenue is concentrated, which stores merit comparison, and what additional evidence management should examine before acting.**

**My approach: Frame the business question. Build a consistent measure. Interpret the result. Recommend the next investigation.**

---

**Khurram Naveed | Data Analyst**

[GitHub](https://github.com/khurraminsights) · [LinkedIn](https://www.linkedin.com/in/khurram-naveed-0083851aa/)

*Independent portfolio case study using simulated retail data; not official reporting for Stylo Pakistan.*

