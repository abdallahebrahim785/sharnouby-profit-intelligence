# 📊 Sharnouby Group — Profit Intelligence Dashboard

> An end-to-end Data Science project analyzing an Egyptian Textile & Apparel company, delivering **22M EGP in actionable profit opportunities** through a 4-page interactive Power BI dashboard.

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 🎯 Project Overview

This project analyzes **3 years of sales data** (Oct 2023 – Sep 2026) from **El-Sharnouby Group**, an Egyptian textile & apparel company based in Alexandria. The analysis identifies critical business risks and delivers **6 strategic recommendations** with an estimated impact of **+22M EGP** in profit.

### 🏢 Business Context
- **Company:** El-Sharnouby Group (Textile & Apparel)
- **Industry:** Manufacturing, Printing, Retail (B2B + B2C)
- **Location:** Alexandria, Egypt
- **Business Units:** Leo Tex, Leo Design, Leo Print, Leo Production Hub, Leo Moda

### 📊 Data at a Glance
| Metric | Value |
|---|---|
| **Total Transactions** | 180,000 |
| **Unique Customers** | 25,634 |
| **Unique Products** | 59 |
| **Time Period** | Oct 2023 – Sep 2026 (36 months) |
| **Total Revenue** | 421.3M EGP |
| **Total Profit** | 64.9M EGP |
| **Overall Margin** | 15.4% |

---

## 🔍 Key Insights

The analysis uncovered **5 critical findings** that shape the business strategy:

### 1. 🚨 Channel Concentration Risk
> **Wholesale generates 85% of total revenue (359M EGP) but only 11.9% profit margin** — while Online & Retail deliver 35–37% margin.

### 2. 💎 Customer Concentration Risk
> **Just 16% of customers (4,200 Champions) drive 78% of revenue** (326.8M EGP). Losing the top 10% would cost ~32M EGP.

### 3. ⚠️ At Risk Customer Base
> **5,349 previously-active customers** (21% of base) haven't purchased in 8+ months, representing **33.6M EGP at risk**.

### 4. 💸 Discount Erosion
> **Discounts above 30% reduce profit margin from 41% to just 8%**, eroding an estimated **2.1M EGP** annually.

### 5. 📍 Geographic Concentration
> **75% of revenue comes from just 5 governorates** (Alexandria alone contributes 29%).

---

## 💡 Strategic Recommendations

Six data-driven recommendations ranked by **impact** and **effort**:

| Priority | Recommendation | Impact (EGP) | Category |
|---|---|---|---|
| 🔴 **High** | Shift 10% of Wholesale volume to Online channel | **+10,000,000** | Channel |
| 🔴 **High** | Launch At Risk customer recovery campaign (5,349 customers) | **+6,700,000** | Customer |
| 🟠 **Medium** | Champion Loyalty Program (4,200 customers) | **+5,000,000** | Customer |
| 🟠 **Medium** | Reduce discounts above 30% on T-Shirts | **+2,100,000** | Pricing |
| 🔵 **Low** | Increase Sweatshirts production (17.9% margin) | **+3,000,000** | Product |
| 🔵 **Low** | Discontinue/Reprice Boys' Beige (loss-making) | **+57,000** | Product |
| | **TOTAL OPPORTUNITY** | **+26,857,000** | |

### 📈 Expected Impact

```text
Current Profit:      64.9M EGP
Target Profit:       91.7M EGP
Total Opportunity:   +26.9M EGP
Growth Rate:         +41%
```


---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| **Data Processing** | Python 3.10+, Pandas, NumPy |
| **Analysis** | Jupyter Notebook, RFM Segmentation, Pareto Analysis |
| **Visualization** | Power BI Desktop, DAX |
| **Data Modeling** | Star Schema (Fact + Dimensions) |
| **Deployment** | Power BI Service |

---

## 📁 Project Structure

```text
sharnouby-profit-intelligence/
│
├── README.md
├── .gitignore
│
├── data/
│   ├── raw/                    # Original CSVs (20 files)
│   └── processed/              # Cleaned & merged data
│
├── notebooks/
│   └── eda.ipynb               # Complete analysis notebook
│
├── powerbi/
│   ├── fact_sales.csv
│   ├── dim_customer.csv
│   ├── dim_product.csv
│   ├── dim_location.csv
│   └── dim_date.csv
│
├── dashboard/
│   ├── Sharnouby_analysis.pbix
│   └── dashboard_screenshots/
│       ├── page1_overview.png
│       ├── page2_customer.png
│       ├── page3_channel.png
│       └── page4_intelligence.png
│
└── docs/
    ├── HVIA_TASK02.pdf
    └── insights_report.md
```

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR-USERNAME/sharnouby-profit-intelligence.git
cd sharnouby-profit-intelligence
```

### 2. Install Python Dependencies
```bash
pip install pandas numpy jupyter matplotlib seaborn
```

### 3. Open the Analysis Notebook
```bash
jupyter notebook notebooks/eda.ipynb
```

### 4. Open the Power BI Dashboard
1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
2. Open `dashboard/Sharnouby_analysis.pbix`.

---

## 🔗 Live Dashboard

🌐 [View Interactive Dashboard on Power BI](https://app.powerbi.com/groups/me/reports/b07950b1-a282-47f9-b6d9-a06ba6508ac1/ca8ee27cf16ac3932df7?experience=power-bi)

> ⚠️ **Note:** The live dashboard requires a Power BI account. For a quick preview, see the screenshots in `/dashboard/dashboard_screenshots`.

---

## 📈 Analysis Methodology

### Phase 1: Data Preparation
- Loaded 20 CSV files (fact + dimensions).
- Cleaned missing values, duplicates, and data types.
- Converted date columns to `datetime` format.
- Built a `sales_master` table by joining facts with dimensions.

### Phase 2: Exploratory Data Analysis (EDA)
- Descriptive statistics on revenue, profit, margin.
- Time series analysis (monthly trends, seasonality).
- Channel & geographic distribution analysis.

### Phase 3: Business Scenarios
Executed 4 analytical scenarios:
1. **Product & Profitability** — Identified top/bottom products, loss-making items, discount impact.
2. **Customer RFM** — Segmented customers into 7 groups (Champions, Loyal, At Risk, Lost, etc.).
3. **Production & Quality** *(optional)* — Production bottlenecks, defect analysis.
4. **Channel & Location** — Channel margin comparison, geographic concentration.

### Phase 4: Dashboard Development
- Built a star schema in Power BI.
- Created 20+ DAX measures (Revenue, Profit, Margin %, Share %, RFM counts, etc.).
- Designed 4 interactive pages with filters and drill-throughs.

### Phase 5: Recommendations
- Ranked recommendations by impact vs. effort.
- Estimated financial impact for each action.

---

## 📊 Key DAX Measures

```dax
-- Total Revenue
Total Revenue = SUM(fact_sales[net_sales_egp])

-- Total Profit
Total Profit = SUM(fact_sales[gross_profit_egp])

-- Profit Margin %
Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)

-- Champion Share %
Champion Share % =
DIVIDE(
    CALCULATE([Total Revenue], dim_customer[segment] = "Champions"),
    [Total Revenue],
    0
)

-- Wholesale Share %
Wholesale Share % =
DIVIDE(
    CALCULATE([Total Revenue], dim_location[channel] = "Wholesale"),
    [Total Revenue],
    0
)

-- At Risk Customers
At Risk Customers =
CALCULATE(
    DISTINCTCOUNT(dim_customer[customer_id]),
    dim_customer[segment] = "At Risk"
)
```

---

## 🎓 Skills Demonstrated

- ✅ Data Cleaning & Wrangling (Pandas)
- ✅ Exploratory Data Analysis (EDA)
- ✅ Feature Engineering (date features, RFM scores)
- ✅ Customer Segmentation (RFM Analysis)
- ✅ Business Intelligence (KPI design)
- ✅ Data Modeling (Star Schema)
- ✅ DAX Programming
- ✅ Dashboard Design (UX/UI)
- ✅ Storytelling with Data
- ✅ Business Recommendations

---

## 📚 Data Sources

| Source | Type |
|---|---|
| El-Sharnouby Group official website | Public |
| Sales transactions | Modeled/Anonymized |
| Customer data | Modeled/Anonymized |
| Product catalog | Public + Modeled |
| Production & operations | Modeled |

*Note: Data was modeled for training/educational purposes. Personal identifiers have been anonymized.*

---

## 👤 Author

**Abdallah Ibrahim**
- 🎓 Data Science Student
- 💼 [LinkedIn](https://www.linkedin.com/in/abdallah-ibrahim-mohamed-4556792a5)
- 🐙 [GitHub](https://github.com/abdallahebrahim785)
- 📧 [your.email@example.com](abdallahebrahim785@gmail.com)

---

## 🙏 Acknowledgments

- **El-Sharnouby Group** for the business context
- **HVIA Data & AI Solutions** for the challenge
- **Olist Dataset** for the analysis framework inspiration

---

## 📄 License

This project is for educational and portfolio purposes. All company data is modeled and anonymized.

---

## ⭐ Support

If you found this project useful, please star ⭐ the repository!

*Built with ❤️ using Python, Pandas, and Power BI*
