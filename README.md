# 💼 SATTVA InfoTech — Internship Portfolio

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=flat-square&logo=python)](https://python.org)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://mysql.com)
[![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=flat-square&logo=pandas)](https://pandas.pydata.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

> **Role:** Python Developer Intern · **Company:** SATTVA InfoTech Pvt. Ltd., Tirupati, India · **Period:** June–August 2023

This repository documents the three core projects delivered during my internship — each solving a real business problem and delivering measurable impact.

---

## 🏆 Impact Summary

| Project | Business Problem | Solution | Measurable Result |
|---------|-----------------|----------|------------------|
| ETL Pipeline | Manual data entry across 3 systems taking 2–3 hrs/day | Automated Python ETL pipeline | **~30% time reduction, zero errors** |
| SQL Optimisation | Queries taking 45–120 seconds on 50K+ records | Schema redesign + targeted indexes | **~25% faster query execution** |
| Report Automation | Manual Excel reports emailed 3hrs late each morning | Automated daily HTML email reports | **2.5 hrs/day saved, zero-error** |

---

## 🏗️ Project Structure

```
8_sattva_internship_portfolio/
│
├── etl/
│   └── etl_pipeline.py              # Extract → Transform → Load automation
│       ├── DataExtractor            # CSV, SQL, JSON, Excel source connectors
│       ├── DataTransformer          # Deduplication, validation, enrichment
│       └── DataLoader               # MySQL/SQLite writer + CSV export
│
├── sql/
│   └── schema_and_queries.sql       # Production schema + 5 optimised queries
│       ├── Schema design            # Normalised tables + FK relationships
│       ├── Indexes                  # 9 targeted indexes for query optimisation
│       └── Optimised Queries        # Monthly revenue, sales performance, CLV, etc.
│
├── automation/
│   └── report_generator.py          # Daily HTML report auto-generated at 8am
│       ├── KPI computation          # Revenue, collection rate, overdue aging
│       ├── Chart generation         # Matplotlib charts embedded in email
│       └── HTML email builder       # Responsive management dashboard email
│
└── requirements.txt
```

---

## 🛠️ Tech Stack

| Area | Technologies |
|------|-------------|
| Language | Python 3.9 |
| Data Processing | Pandas, NumPy |
| Database | MySQL 8.0 (SQLite for local demo) |
| Automation | Python cron scheduling, SQLAlchemy |
| Visualisation | Matplotlib, Seaborn |
| Email | smtplib, MIME (HTML emails) |

---

## 🚀 Quick Start

```bash
git clone https://github.com/sahil-mali19/sattva-internship-portfolio.git
cd sattva-internship-portfolio
pip install -r requirements.txt

# Run ETL pipeline (generates clean database)
python etl/etl_pipeline.py

# Generate daily report
python automation/report_generator.py

# Preview KPIs only
python automation/report_generator.py --preview
```

---

## 📋 ETL Pipeline Detail

### Data Sources Processed
| Source | Format | Records/Week |
|--------|--------|-------------|
| CRM System | MySQL DB | ~5,000 |
| Billing System | CSV export | ~8,000 |
| Inventory System | REST API (JSON) | ~12,000 |

### Cleaning Operations Applied
- Exact and flagged duplicate removal
- Email validation and filtering
- Mixed-format number parsing (₹1,234 / 1234.56 / 1,234.56)
- Missing value imputation (median by group)
- Date standardisation (multiple input formats → ISO 8601)
- Feature engineering (CLV tier, recency, overdue aging)

---

## 📊 SQL Queries Included

1. **Monthly Revenue Report** — management KPI dashboard query
2. **Sales Rep Performance Scorecard** — individual performance ranking
3. **Customer Lifetime Value (CLV)** — top 50 by lifetime spend
4. **Overdue Collection Priority** — aging buckets + recommended actions
5. **Regional & Industry Revenue** — cross-dimensional revenue analysis

---

## 👤 Author
**Sahil Mali** | MSc Business Analysis & Consulting — University of Strathclyde  
📧 sahil06june2003@gmail.com | 🔗 [LinkedIn](https://linkedin.com/in/sahil-mali-2755021b9)
