# Road Accident Analysis — Real‑World Data Analysis Report

## 🔎 Project Overview
This notebook analyzes road‑accident records to uncover patterns, data quality issues, and category‑level distributions. The goal is to demonstrate a clean, end‑to‑end analytics workflow — **data loading → cleaning → feature engineering → EDA → insights** — suitable for decision‑making and portfolio showcasing.

## 🧰 Tools & Libraries
- Python (3.10+)
- Jupyter Notebook
- pandas
- matplotlib

### Data Quality
- Duplicate **rows**: **0**
- Duplicate **IDs** (`Accident_Index`): **0**
- Top missing fields:
  - `Time`: 17 missing (0.01%)
  - `Carriageway_Hazards`: 3 missing (0.0%)
  - `Accident_Index`: 0 missing (0.0%)
  - `Number_of_Casualties`: 0 missing (0.0%)
  - `Weather_Conditions`: 0 missing (0.0%)
  - `Urban_or_Rural_Area`: 0 missing (0.0%)
  - `Speed_limit`: 0 missing (0.0%)
  - `Road_Type`: 0 missing (0.0%)

## 🧪 Method (Notebook Workflow)
1. Load CSV and inspect shape/dtypes
2. Parse date/time and create features: `year`, `month = dt.month_name()`, `hour`
3. Handle data quality: trim text, fix types, address nulls/duplicates
4. Exploratory analysis: monthly/hourly trends, category distributions
5. Visualize with clear titles, labels, tick rotation, and grids

## 🔍 Insights (Key Findings)
- **Seasonality (by month):** Top months by incidents → **November** (29094); **October** (28368); **July** (26952).
- **Rush‑hour pattern (by hour):** Peak hours → **17:00** (26964); **16:00** (24903); **15:00** (24151).
- **Accident_Severity split:** **Slight** (263280); **Serious** (40740); **Fatal** (3904); **Fetal** (49).
- **Light_Conditions split:** **Daylight** (227286); **Darkness - lights lit** (60093); **Darkness - no lighting** (16528); **Darkness - lighting unknown** (2924); **Darkness - lights unlit** (1142).
- **Road_Surface_Conditions split:** **Dry** (208967); **Wet or damp** (81796); **Frost or ice** (12078); **Snow** (4758); **Flood over 3cm. deep** (374).



## 🧾 Brief Summary
- 307973 records across 21 fields | covering 2021-01-01 to 2022-12-31 | top month(s): November, October, July | peak hour(s): 17:00, 16:00, 15:00.
- Clean workflow with feature engineering (month names, hours) and clear visuals demonstrates strong EDA skills.



