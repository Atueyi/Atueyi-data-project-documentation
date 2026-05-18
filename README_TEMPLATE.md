# OnePort365 Freight & Performance Analytics Dashboard

> A Power BI dashboard designed to analyze global freight operations, shipment performance, carrier efficiency, and commodity-based revenue trends to support logistics decision-making and operational visibility.

---

## ⚙️ Project Type Flags

- [ ] Dashboard / Data Visualization
- [ ] Data Cleaning / Wrangling
- [ ] End-to-End
- [ ] Business Intelligence Reporting

---

# Table of Contents

1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Repository Structure](#4-repository-structure)
5. [Data Workflow](#5-data-workflow)
6. [Data Model & Schema](#6-data-model--schema)
7. [Analysis & Metrics](#7-analysis--metrics)
8. [Key Insights](#8-key-insights)
9. [Recommendations](#9-recommendations)
10. [Assumptions & Limitations](#10-assumptions--limitations)
11. [Future Enhancements](#11-future-enhancements)
12. [Deliverables](#12-deliverables)
13. [Author](#13-author)

---

# 1. Project Overview

### Context
Freight and logistics companies require visibility into shipment efficiency, vessel reliability, delivery timelines, and revenue performance across international trade routes. Managing these operations manually can make it difficult to identify delays, underperforming carriers, and high-value shipment patterns.

### Problem Statement
The business needed a centralized reporting solution to monitor shipment operations, track delivery performance, evaluate carrier reliability, and analyze commodity-level freight revenue trends.

### Approach
Using Power BI, shipment and freight data were cleaned, transformed, and modeled into an interactive dashboard solution. Multiple analytical pages were created to monitor operational KPIs, SLA performance, vessel efficiency, and commodity revenue distribution.

### Outcome
The project produced a multi-page business intelligence dashboard that provides operational visibility into freight performance, shipment delays, cancellations, carrier reliability, and revenue-driving commodities across global shipping destinations.

---

# 2. Objectives

- **Primary Objective:** Build an interactive freight analytics dashboard for monitoring shipment operations and logistics performance.

- **Secondary Objective 1:** Identify shipment delay patterns and evaluate on-time delivery performance.

- **Secondary Objective 2:** Analyze vessel and carrier efficiency across international destinations.

- **Secondary Objective 3:** Evaluate freight revenue trends and high-performing commodity categories.

> 💡 Every analysis decision in this project was designed to improve operational visibility and support logistics decision-making.

---

# 3. Project Scope & Tools

## Scope

| Dimension | Details |
|-----------|---------|
| **In Scope** | Shipment performance, freight revenue, vessel performance, carrier reliability, commodity analysis, destination-country trends |
| **Out of Scope** | Customer behavioral analysis, predictive forecasting, warehouse inventory analysis |
| **Time Period** | January 2023 – December 2024 |
| **Granularity** | Shipment-level and aggregated operational metrics |

---

## Tools & Technologies

| Category | Tool(s) Used |
|----------|-------------|
| Data Storage | Excel / CSV Data Sources |
| Data Processing | Power Query |
| Analysis | DAX Measures & Calculations |
| Visualization | Power BI |
| Version Control | Git & GitHub |
| Documentation | Markdown |

---

# 4. Repository Structure

```bash
project-root/
│
├── data/
│
├── visuals/
│   ├── executive_overview.png
│   ├── operations_sla.png
│   ├── vessel_performance.png
│   └── finance_commodity.png
│
├── reports/
│
├── OnePort365_Freight_Dashboard.pbix
│
└── README.md
```

---

# 5. Data Workflow

```text
[Freight & Shipment Data]
        ↓
[Data Import into Power BI]
        ↓
[Cleaning & Transformation using Power Query]
        ↓
[DAX Calculations & KPI Creation]
        ↓
[Dashboard Visualisation & Reporting]
```

### 1. Source
Freight shipment datasets containing shipment details, destination countries, vessel information, TEUs, freight revenue, delays, and shipment statuses.

### 2. Ingestion
Data was imported into Power BI from structured tabular datasets.

### 3. Cleaning
Data formatting issues, inconsistencies, and missing values were handled using Power Query transformations.

### 4. Transformation
Calculated metrics such as:
- On-time delivery rate
- Average delay days
- Freight per TEU
- Cancellation rate
- Commodity-level revenue contribution

### 5. Analysis
Descriptive and operational analysis was performed using KPI cards, trend charts, vessel comparisons, and commodity segmentation.

### 6. Output
An interactive multi-page Power BI dashboard for operational monitoring and executive reporting.

---

# 6. Data Model & Schema

## Dataset: Freight Shipment Data

| Field Name | Data Type | Description | Example Value |
|------------|-----------|-------------|---------------|
| Shipment_ID | Integer | Unique shipment identifier | 10245 |
| Destination_Country | String | Shipment destination country | Netherlands |
| Vessel_Name | String | Name of shipping vessel | ONE Apus |
| Shipping_Line | String | Carrier/shipping company | Maersk |
| Freight_USD | Decimal | Freight value in USD | 950,000 |
| TEUs | Integer | Twenty-foot Equivalent Units | 850 |
| Delay_Days | Decimal | Shipment delay duration | 5.4 |
| Shipment_Status | String | Shipment delivery status | Delayed |
| Commodity | String | Product/commodity category | Electronics |
| Shipment_Date | Date | Shipment transaction date | 2024-05-12 |

> **Row count (approx.):** 2,385 shipments  
> **Date range:** Jan 2023 – Dec 2024

---

# 7. Analysis & Metrics

## Analytical Approach

The analysis focused on operational monitoring and logistics performance evaluation. KPI tracking, trend analysis, carrier comparisons, and commodity segmentation were used to identify operational inefficiencies and revenue-driving patterns.

---

## Key Metrics Defined

| Metric | Plain-Language Definition | Why It Matters |
|--------|--------------------------|----------------|
| Total Shipments | Total number of processed shipments | Measures operational volume |
| Total Freight (USD) | Total freight revenue generated | Measures business performance |
| On-Time Rate | Percentage of shipments delivered on time | Measures operational efficiency |
| Average Delay (Days) | Average shipment delay duration | Identifies SLA performance gaps |
| Cancellation Rate | Percentage of cancelled shipments | Measures operational reliability |
| Freight per TEU | Average freight revenue earned per TEU | Evaluates shipment profitability |

---

## Methods Used

- KPI Monitoring
- Trend Analysis
- Comparative Vessel Analysis
- Commodity Revenue Segmentation
- Freight Distribution Analysis
- Operational Performance Evaluation

---

# 8. Key Insights

## Insight 1: Freight Revenue Exceeded $61M

The dashboard revealed total freight revenue of approximately **$61.7M** generated across **2,385 shipments**, indicating strong operational throughput and global shipping activity.

---

## Insight 2: On-Time Performance Requires Improvement

Despite high shipment volume, the overall on-time delivery rate was approximately **52.54%**, highlighting operational inefficiencies and possible SLA compliance challenges.

---

## Insight 3: Certain Ports Experience Significant Delays

Mumbai and Shanghai recorded some of the highest shipment transit delays, suggesting potential congestion or operational bottlenecks within these shipping routes.

---

## Insight 4: Electronics and Automobiles Drive Freight Revenue

Electronics and automobile shipments contributed the highest freight revenue, each generating over **$6.6M**, making them the most commercially valuable commodity categories.

---

## Insight 5: Vessel Performance Varies Significantly

Vessels such as **ONE Apus** and **Maersk Alabama** achieved the strongest on-time performance, while others showed lower delivery consistency.

---

# 9. Recommendations

| Priority | Recommendation | Based On | Suggested Owner |
|----------|---------------|----------|-----------------|
| High | Investigate operational bottlenecks affecting delayed shipment routes | High average delays | Operations Team |
| High | Improve SLA monitoring for underperforming shipping lines | Low on-time delivery rate | Logistics Management |
| Medium | Increase focus on high-performing commodity categories | Commodity revenue trends | Commercial Team |
| Medium | Optimize shipment planning for high-delay ports | Port delay analysis | Supply Chain Team |
| Low | Develop predictive delay monitoring dashboards | Current reporting limitations | BI & Analytics Team |

---

# 10. Assumptions & Limitations

## Assumptions

- Shipment records were assumed to be complete and accurate.
- Freight values were assumed to be reported consistently across all regions.
- Delay calculations were based on available shipment timestamps.

---

## Limitations

- External factors such as weather, customs delays, and geopolitical disruptions were not included.
- The dashboard does not include predictive forecasting models.
- Real-time shipment tracking integration was outside project scope.
- Some map visuals were disabled due to Power BI security settings.

---

# 11. Future Enhancements

- [ ] Integrate real-time shipment tracking APIs
- [ ] Add predictive delay forecasting models
- [ ] Build automated refresh pipelines
- [ ] Add regional profitability analysis
- [ ] Include customer-level shipment analytics

---

# 12. Deliverables

| Deliverable | Description | Location |
|-------------|-------------|----------|
| Power BI Dashboard | Interactive freight analytics dashboard | `/OnePort365_Freight_Dashboard.pbix` |
| Dashboard Screenshots | Exported dashboard visuals | `/visuals/` |
| Project Documentation | GitHub README documentation | `/README.md` |

---

# 13. Author

**Ebube Atueyi**  
Data Analyst | Power BI Developer | Business Intelligence Analyst

- 🔗 LinkedIn: www.linkedin.com/in/ebube-atueyi-4a487623a
- 💼 GitHub: https://github.com/Atueyi

---

*Last updated: May 2026*
