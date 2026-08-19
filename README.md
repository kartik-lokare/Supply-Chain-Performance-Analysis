
# 🧾 Supply Chain Performance Analysis
_Analyzing Supply Chain efficiency and profitability to support inventory decisions using Python, and Power BI._

---

## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
- <a href="#dashboard">Dashboard</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>
- <a href="#author--contact">Author & Contact</a>

---
<h2><a class="anchor" id="overview"></a>Overview</h2>

This project is provide a comprehensive overview of key supply chain operations, enabling businesses to monitor performance and make data-driven decisions. 

---
<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

A manufacturing and distribution company is facing delays in deliveries, inconsistent vendor performance, excess inventory in some warehouses, and frequent order processing issues. Management lacks a centralized dashboard to monitor the complete supply chain performance.This project aims to:
- Improve inventory visibility and stock management.
- Monitor on-time delivery performance across regions.
- Evaluate vendor performance and supplier reliability.
- Track order status for better operational control.
- Enable data-driven decision-making through interactive dashboards

---
<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- excel files located in `/data/` folder (sales, vendors, inventory)

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- Python (Pandas, Matplotlib, Seaborn)
- Power BI (Interactive Visualizations)
- Excel
- GitHub

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
vendor-performance-analysis/
│
├── README.md
├── .gitignore
├── requirements.txt
├── Vendor Performance Report.pdf
│
├── notebooks/                  # Jupyter notebooks
│   └── Supply Chain Notebook.ipynb
│
├── dashboard/                  # Power BI dashboard file
│   └── Supply Chain Dashboard.pbix
```

---
<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

- **Total Sales: Rs 28,71,52,741 | Total Profit: Rs 4,73,86,540 | Overall Margin: 16.5%**
- On-time delivery rate is only ~38.8% — the majority of orders (61.2%) are delayed, a significant operational concern
- Order Status is split almost evenly — 34.1% Cancelled, 33.1% Delivered, 32.8% Pending — an unusually high cancellation rate worth investigating
- No orders show negative profit — unlike typical retail data, this dataset has no loss-making transactions, which is worth validating against the       data source
- No missing values and no duplicate records — the dataset is clean and ready for further modeling
- Vendor 7 has the best on-time rate (41.6%), while Vendor 10 has the worst (35.8%) — despite both carrying identical average ratings (4.0),             reinforcing that rating alone isn't a good delivery predictor
- **Suggested Next Steps**
- Investigate root causes of delays — 61% delayed is high; break down by lead time bucket, warehouse, or vendor
- Reduce cancellations — a ~34% cancellation rate is unusually high; check if it's tied to stockouts or specific categories
- Revisit vendor scoring — since rating doesn't predict on-time performance, consider adding delivery-based KPIs
- Tighten reorder policies — 12% of orders sit at/below reorder level; review reorder thresholds by category
- Validate the "zero loss orders" finding — confirm this reflects real business rules and isn't a data-generation artifact

---

---
<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

- Power BI Dashboard shows:
  - Inventory by Warehouse
  - Inventory status
  - Avg Delivery Time
  - Performance

![Vendor Performance Dashboard](images/dashboard.png)

---
<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

1. Clone the repository:
```bash
git clone https://github.com/yourusername/vendor-performance-analysis.git
```
2. Open and run notebooks:
   - `notebooks/Supply Chain Notebook.ipynb`
3. Open Power BI Dashboard:
   - `dashboard/Supply Chain Dashboard.pbix`

---
<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>

- Maintain optimal inventory levels by replenishing low-stock products and reducing excess inventory.
- Improve delivery planning in regions with lower on-time delivery performance.
- Work closely with low-performing vendors to improve delivery reliability and service quality.
- Prioritize pending orders to reduce delays and enhance customer satisfaction.
- Investigate cancelled orders to identify root causes and minimize future cancellations.

---
<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

**Kartik Lokare**  
Data Analyst  
📧 Email:[kartiklokare8@gmali.com](kartiklokare8@gmali.com)
🔗 [LinkedIn](linkedin.com/in/kartik-lokare-5521a7395)  
