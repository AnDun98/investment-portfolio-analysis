# Data Processing

## Overview
This folder contains the Jupyter Notebook for Block 1 - data quality audit and cleaning.

## What the Notebook Does
The notebook is structured as a sequential pipeline with sections:
Section | Content
--- | ---
0 | Data loading and initial overview
1 | Defect 1: Duplicate and missing Projects IDs
2 | Defect 2: Mixed date formats (datetime vs text string)
3 | Defect 3: Status field typo standardisation
4 | Defect 4: Technical dates
5 | Defect 5: Missing launch dates - completeness analysis and critical cases
6 | Defect 6: Empty Functional Area field
7 | Defect 7: Additional anomalies (zero budgets, early forecast dates, single completed project)
8 | Export cleaned dataset to data_cleaned.xlsx
