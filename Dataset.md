# 🗄️ Dataset Overview: IPL Complete Dataset (2008–2024)

**Source:** [Kaggle - IPL Complete Dataset (2008-2024)](https://www.kaggle.com/datasets)

To ensure this repository remains lightweight and performs optimally, the raw `.csv` data files are not hosted directly in this folder.

### 📊 Data Scale & Scope
* **Time Period:** 16 seasons (2008–2024)
* **Match-level records:** ~1,095 matches
* **Ball-by-ball transaction records:** 260,000+ deliveries
* **Format:** Two relational CSVs (match-level dimension table + delivery-level fact table)

### 🗂️ Table Schema
The data was modeled and joined within Tableau:
1. `matches.csv` (Match-level dimension table — teams, toss, venue, result, season)
2. `deliveries.csv` (Ball-by-ball fact table — joined to matches on Match ID)

Both tables were joined on **Match ID**, then restructured into a team-centric analytical model (see documentation) to enable accurate team-level filtering across the dashboard.
