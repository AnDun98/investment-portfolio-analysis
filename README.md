# 📊 Investment Portfolio Analysis

# 📌 Overview
This project presents an end-to-end analysis of a corporate investment project portfolio. The work covers data quality assessment and cleaning, interactive dashboard development and business insights with actionable recommendations.

## Key findings at a glance:
- Portfolio of 1,595 projects with a total approved budget of **676.7B RUB**
- Forecast budget exceeds approved by **+82.9%** (+561.3B RUB)
- **51% of projects with known dates are delayed** - average delay 407 days
- **22% of projects are on hold** (357 out of 1,595)
- Average PM workload: **41 active projects per manager** (max 57)

---

## ⚙️ Block 1 - Data Preparation
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

**Result:** 1,595 clean records saved to data_cleaned.xlsx
---

## 🛠️ Tech Stack
- Python (pandas, numpy)
- Power BI
