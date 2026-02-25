# 📦 Supply Chain Performance Dashboard | Power BI

An end-to-end **Supply Chain Analytics Dashboard** built in Power BI, covering executive-level KPIs, operations & production performance, and logistics & quality analysis across three interactive report pages.
The objective was to design a business-ready dashboard that delivers actionable insights for executive decision-making.

The dashboard focuses on:
  - Financial performance analysis
  - Supplier risk identification
  - Logistics cost optimization
  - Quality performance monitoring
    
---

## 📊 Dashboard Overview

This dashboard provides a 360° view of supply chain performance across **5 suppliers**, **3 product types** (Skincare, Haircare, Cosmetics), and **4 transportation modes** (Road, Rail, Air, Sea). It is designed to support data-driven decisions in procurement, logistics, and production management.

### Pages

| Page | Description |
|------|-------------|
| **Executive Overview** | High-level KPIs: Revenue, Cost, Profit, Lead Time, Defect Rate |
| **Operations & Production Performance Analysis** | Supplier comparison by lead time, defect rate, and production volume |
| **Logistics & Quality Performance Analysis** | Transportation mode analysis, route performance, inspection results |

---

## 🗂️ Project Structure

```
supply-chain-dashboard/
│
├── SupplyChainDashboard.pbix       # Main Power BI file
├── data/
│   └── supply_chain_data.csv       # Source dataset
├── screenshots/
│   ├── executive_overview.png
│   ├── ops_production.png
│   └── logistics_quality.png
└── README.md
```

---

## 📌 Key Metrics & KPIs

### Executive Overview
| KPI | Value |
|-----|-------|
| Total Revenue | $577.60K |
| Total Cost | $57.65K |
| Net Profit | $519.95K |
| Profit Margin % | 90.02% |
| Avg Lead Time | 17.08 days |
| Avg Defect Rate | 2.28% |

### Operations & Production
| KPI | Value |
|-----|-------|
| Total Production Volume | 57K units |
| Avg Manufacturing Lead Time | 14.77 days |
| Highest Risk Supplier | Supplier 5 |

### Logistics & Quality
| KPI | Value |
|-----|-------|
| Total Transportation Cost | $52.92K |
| Highest Risk Transport Mode | Road |
| Inspection Pass Rate | 41% |
| Inspection Fail Rate | 36% |
| Inspection Pending | 23% |

---

## 🔍 Dashboard Pages — Detailed Breakdown

### 1. Executive Overview
- **Revenue & Profit by Product Type** — Skincare leads in absolute profit ($217K), followed by Haircare ($155K) and Cosmetics ($147K). All three maintain ~90% profit margins.
- **Risk Scatter Plot** — Haircare carries the highest operational risk (highest lead time + defect rate combo), while Cosmetics is the most operationally efficient product line.
- **Summary Table** — Tabular breakdown of Revenue, Cost, Net Profit, Profit Margin, Avg Defect Rate, and Avg Lead Time by product type.

**Key Insight:** Cosmetics is operationally efficient but commercially underperforming relative to its potential.

---

### 2. Ops & Production Performance Analysis
- **Production Volume by Product Type** — Skincare (24K) > Haircare (20K) > Cosmetics (12K), creating concentration risk.
- **Avg Manufacturing Lead Time by Supplier** — Supplier 5 has the longest lead time (16.33 days); Supplier 1 is the fastest (12.59 days).
- **Supplier Risk Matrix (Scatter)** — Supplier 5 is a clear outlier with high lead time AND high defect rate. Supplier 1 is the top performer on both dimensions.
- **Supplier Summary Table** (sorted by defect rate):

| Supplier | Avg Mfg Lead Time | Avg Defect Rate | Production Volume | Mfg Cost |
|----------|-------------------|-----------------|-------------------|----------|
| Supplier 5 | 16.33 | 2.67 | 9,381 | 805.83 |
| Supplier 3 | 14.93 | 2.47 | 7,997 | 654.51 |
| Supplier 2 | 15.59 | 2.36 | 14,105 | 915.70 |
| Supplier 4 | 15.33 | 2.34 | 11,756 | 1,128.78 |
| Supplier 1 | 12.59 | 1.80 | 13,545 | 1,221.86 |

**Key Insight:** Supplier 1 consistently outperforms on efficiency and quality. Supplier 5 requires immediate performance remediation.

---

### 3. Logistics & Quality Performance Analysis
- **Transportation Cost by Mode** — Road ($16K) is costliest, followed by Rail ($15.2K), Air ($14.6K), Sea ($7.1K).
- **Avg Lead Time by Mode** — Road is slowest (18 days); Air is fastest (16 days).
- **Defect Rate by Mode** — Road has the highest defect rate (2.62); Air has the lowest (1.82).
- **Route Analysis** — Route B has the highest avg lead time (18.2 days) and highest total cost ($22K).
- **Inspection Results** — Only 41% of inspections pass; 36% fail and 23% remain pending — a significant quality backlog.

**Key Insight:** Road transportation is the highest cost, slowest, and most defect-prone mode. Shifting volume to Air is recommended for high-value, time-sensitive shipments.

---

## 💡 Strategic Recommendations

1. **Reduce Road transport dependency** — Road carries the highest cost, defect exposure, and lead times simultaneously.
2. **Expand Supplier 1 allocation** — Supplier 1 is the best performer across all operational metrics and can absorb more volume.
3. **Initiate corrective action for Supplier 5** — Supplier 5 represents the highest operational risk and needs a formal improvement plan or contract review.
4. **Resolve the inspection backlog** — A 23% pending rate signals a process bottleneck that could mask further quality failures.
5. **Optimize Route B** — Route B concentrates both delay and cost; routing alternatives should be explored.
6. **Diversify Skincare production** — Skincare represents 42% of total volume, creating an operational concentration risk.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** — Report development, DAX measures, data modelling, Conditional Formatting, Interactive slicers
- **DAX** — Custom KPI calculations (Profit Margin %, Avg Defect Rate, Avg Lead Time, risk flags)
- **Power Query (M)** — Data transformation and cleaning
- **Data Source** — CSV supply chain dataset

---

## 🎛️ Filters & Slicers

Each page includes interactive slicers to drill down by:
- **Product Type** (Skincare, Haircare, Cosmetics)
- **Supplier Name** (Supplier 1–5)
- **Transportation Mode** (Road, Rail, Air, Sea) *(Logistics page)*

---

## 📸 Screenshots

### Executive Overview
![Executive Overview](screenshots/executive_overview.png)

### Ops & Production Performance
![Ops & Production](screenshots/ops_production.png)

### Logistics & Quality Performance
![Logistics & Quality](screenshots/logistics_quality.png)

---

## 📈 Business Impact

This dashboard enables leadership to:

  - Identify high-risk suppliers
  - Reduce logistics inefficiencies
  - Monitor quality backlog exposure
  - Optimize transport mode allocation
  - Improve cost and performance balance

---

## 🚀 Conclusion

This project demonstrates structured supply chain analytics, combining financial performance, operational diagnostics, and logistics optimization into a cohesive executive dashboard.

The focus was not just on visualization, but on delivering decision-oriented insights.

---

## 🚀 How to Use

1. Clone or download this repository.
2. Open `SupplyChainDashboard.pbix` in **Power BI Desktop**.
3. If prompted, update the data source path to point to `data/supply_chain_data.csv`.
4. Refresh the data and explore all three report pages.
5. Use the slicers on each page to filter by product type, supplier, or transportation mode.

---

## 📬 Contact

Built by Harshitha | https://linkedin.com/in/salianharshitha

---

*Dashboard built with Power BI Desktop. Data is illustrative and used for analytical demonstration purposes.*
