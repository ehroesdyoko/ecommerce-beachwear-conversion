# Ecommerce Beachwear Conversion Analysis

Project Assignment
Objective: Pinpoint the levers that can lift an online fashion retailer’s beachwear conversion rate by ≥ 1 percentage point.

Client identity anonymised as RetailCo for confidentiality.

✨ Project snapshot

A full end‑to‑end data‑engineering and analytics workflow in R that marries:

⚙️ Internal click‑stream & order data from RetailCo (600 k sessions, 2021‑2022)

☀️ KNMI weather metrics (temperature, sunshine, precipitation)

🦠 COVID‑19 case counts (JHU CSSE)

🔍 Google Trends for swim‑related keywords

The analysis tests 11 business hypotheses (demographics, device, seasonality, brand…) and delivers actionable recommendations for RetailCo’s merchandising & marketing teams.

🚀 Quick start

## 🧪 Tools Used

- **R**: Data cleaning, imputation (MICE), statistical modeling, and visualization
- **SQL**: Data extraction
- **Jupyter Notebook**: SQL queries demonstration
- **ggplot2**, **dplyr**, **mice**, **lmtest**, **grangertest**

📄 Data

Source

RetailCo internal (NDA) - Four tables: events, customers, orders, articles — not redistributed. Replace the placeholder script R/02_download_internal.R with your own extract.

KNMI Royal Netherlands Met Institute - Daily weather for NL, 2021‑2022 (public).

JHU CSSE COVID‑19 - Netherlands cumulative cases.

Google Trends - Weekly search interest for swimwear, zwembroek, RetailCo, competitors.

For privacy & size reasons, the repo ships no raw data; only processed, de‑identified summaries live in data/processed/.


📊 Key results

Male shoppers convert at 10.7 % vs 8.4 % for females.

+0.1 °C → +0.011 pp conversion (but effect reverses on consecutive hot days).

Desktop shows highest conversion despite mobile traffic dominance.

See full interpretation and managerial actions in docs/Report.pdf.

🤝 Authors

Erlangga Roesdyoko · Daniel Hsu · Nils Depner · Ruben Meijer 


🙌 Acknowledgements

Thanks to RetailCo for providing the anonymised click‑stream dataset and to KNMI, JHU CSSE, and Google Trends for open data services.

## 📁 Repository Structure

```bash
ecommerce-beachwear-conversion/
│
├── report/
│   └── E-commerce Conversion Report.pdf        # Final written analysis
│
├── SQL/
│   └── SQL - Data Extraction.ipynb             # Raw SQL code + explanation
│
├── R/                                  # (Optional) Add your main R analysis files here
│
├── README.md
└── .gitignore
