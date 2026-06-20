# Dashboard

## Overview
This folder contains the Power BI dashboard for Block 2.

## Dashboard Structure
### Page 1 - Portfolio Overview

Hight-level summary for executive audience.
<img height="800" alt="image" src="https://github.com/user-attachments/assets/f281657d-fc1e-4127-8231-4ed173a9cda0" />

Visual | Description
--- | ---
6 KPI Cards | Total projects, active, on hold, approved budget, forecast budget, overrun %
Donut chart | Project distribution by status
Clustered bar chart | Approved vs forecast budget by programme
Matrix | Office to Status - number of projects with conditional formatting
Slicers | Office, Programme, Category, Status

---

### Page 2 - Budget Analysis

Where and by how much are budgets being exceeded?
<img height="800" alt="image" src="https://github.com/user-attachments/assets/2b7952de-0050-4208-89d9-80d6792a3a5d" />

Visual | Description
--- | ---
Clustered column chart | Approved vs forecast budget by office
Bar chart | Project by overrun range (<= 0%, 0-20%, 20-50%, > 50%)
Table (Top 15) | Projects with highest budget overrun - conditional formatting applied
Column chart | Overrun % by functional area
Slicers | Office, Programme, Category, Status

---

### Page 3 - Schedule Analysis

Which projects are delayed and by how much?
<img height="800" alt="image" src="https://github.com/user-attachments/assets/9eb6a85d-eea0-4e59-b568-019c1a16df31" />

Visual | Description
--- | ---
Bubble chart | Plan vs forecast launch date - bubble size = budget, colour = status
Bar chart | Project by delay range (on time, < 90d, 90-180d, 180-365d, > 365d)
Table (Top 15) | Projects with longest delays - conditional formatting applied
Column chart | Forecast launches by year
Slicers | Office, Programme, Category, Status

---

### Page 4 - Project Managers

Who is managing what and how effectively?
<img height="800" alt="image" src="https://github.com/user-attachments/assets/8e3e847b-d55d-4238-9d41-54091f2f02ce" />

Visual | Description
--- | ---
Table | PM summary: project count, total budget, overrun %, delay days
Bar chart (Top 15) | PMs by number of active projects
Bar chart (Top 10) | PMs by budget overrun %
Slicers | Office, Programme, Category, Status
