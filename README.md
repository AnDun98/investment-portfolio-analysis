# 📊 Investment Portfolio Analysis

# 📌 Overview
This project presents an end-to-end analysis of a corporate investment project portfolio. The work covers data quality assessment and cleaning, interactive dashboard development and business insights with actionable recommendations.

The analysis covers three major areas:
- Data Quality Assessment
- Portfolio Perfoemance Analysis
- Executive Dashboard Development

---

## 🎯 Business Objectives
The purpose of this analysis is to provide management with a consolidated view of the investment portfolio and identify projects requiring increased attention due to budget or schedule risks.

Key business questions:
- What is the current state of the investment portfolio?
- Which projects represent the highest financial risk?
- Where are budget overruns concentrated?
- Which organizational units require management attention?
- What additional information is needed to improve governance?

---

## ⚙️ Dataset
**Source file:** Пуски Бюджет.xlsx - 1,615 rows, 14 columns

**Data Quality Passport**
Column | Completeness | Issues Found | Resolution
--- | --- | --- | ---
Project ID (SPP) | 99.6% | 6 missing, 16 duplicates | Isolated for manual review
Project Status | 100% | Typo 'В архив' vs 'В архиве' | Standardised
Phase | 100% | - | Clean
Category | 100% | - | Clean
Launch Date (Plan) | 48.1% | Mixed format: datetime + string (68 rows) | Unified to datetime
Launch Date (Forecast) | 58.8% | Mixed format: datetime + string (67 rows) | Unified to datetime
Functional Area | 98.2% | 29 nulls + text 'None' | Replaced with 'Not specified'

**Defects Summary**
№ | Defect | Rows Affected | Action Taken
--- | --- | --- | ---
1 | Duplicate / missing SPP codes | 22 | Isolated for source review
2 | Mixed date formats | 68 | Converted to datetime
3 | Status firld typo | 2 | Standardised
4 | Missing launch dates | 646 | Filtered for schedule metrics
5 | Empty functional area | 29 | Filled as 'Not specified'
6 | Only 1 completed project | 1 | Flagged for stakeholder clarification

**✔️ Result:** 1,595 clean records saved to data_cleaned.xlsx

---

## 📈 Block 2 - Dashboard

The dashboard consists of 4 pages:
Page | Purpose
--- | ---
Portfolio Overview | KPI cards, status distribution, budget ny programme, office and status matrix
Budget Analysis | Plan vs Forecast by office, overrun distribution, top-15 projects by overrun
Schedule Analysis | Plan vs Forecast launch dates, delay distribution, top-15 delayed projects, quarterly launch forecast
Project Managers | Workload ranking, budget overrun % per PM, delay % per PM

---

## Dashboard Preview
<img height="800" alt="image" src="https://github.com/user-attachments/assets/3bb04e7e-036f-4d3a-a80d-0f05999ab454" />

---

## 🛠️ Tech Stack
- Python (pandas, numpy)
- Power BI
