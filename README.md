# 🏏 IPL 2025 Mega Auction — Player Targeting Analysis

A data-driven project to build the optimal IPL team for the 2025 Mega Auction using historical performance data (2022–2024) from Kaggle. The analysis removes retained players and identifies high-value targets across batting, bowling, and all-round roles.

---

## 📁 Project Structure

```
Data/
├── Images/
│   ├── All-Rounder Targets.png
│   ├── Batting_Selection(Avg vs SR).png
│   └── Bowling_Selection(Avg vs Econ).png
│
├── Notebook/
│   ├── clean.ipynb              # Data cleaning pipeline
│   ├── mergingdata.ipynb        # Merging deliveries + matches datasets
│   ├── Batting_Selection.ipynb  # Batting analysis & target shortlisting
│   ├── Bowling_Selection.ipynb  # Bowling analysis & target shortlisting
│   └── All_rounders.ipynb       # All-rounder impact scoring
│
├── Raw/
│   ├── deliveries.csv           # Ball-by-ball data (Kaggle IPL dataset)
│   └── matches.csv              # Match-level data (Kaggle IPL dataset)
│
└── Processed/
    ├── matches_clean.csv
    ├── deliveries_clean.csv
    ├── matches_new.csv
    └── merged.csv               # Final merged dataset (generated locally)
```

---

## 🎯 Project Objective

With the IPL 2025 Mega Auction, all teams had to rebuild their squads from scratch (except retained players). This project:

- Analyses **3 seasons of IPL data (2022–2024)**
- Filters out retained/unavailable players
- Identifies the best **available** players by role using stats-based scoring
- Targets players across **openers, middle-order, powerplay bowlers, death bowlers, and all-rounders**

---

## 📊 Analysis & Results

### 🏏 Batting — Average vs Strike Rate

![Batting Selection](Images/Batting_Selection(Avg vs Econ).png)

Batters are scored on a combination of batting average and strike rate over the last 3 IPL seasons. Openers are prioritised for powerplay aggression; middle-order for consistency under pressure.

**Top Targets:** Jake Fraser-McGurk, Phil Salt, Jos Buttler

---

### 🎳 Bowling — Average vs Economy

![Bowling Selection](Images/Bowling_Selection(Avg vs Econ).png)

Bowlers are evaluated on economy rate, wicket-taking ability, and phase-wise performance (powerplay vs death overs).

**Top Targets:** Trent Boult, Mohammed Shami, Bhuvneshwar Kumar, Arshdeep Singh, Mohammed Siraj

---

### ⚡ All-Rounders — Impact Score

![All-Rounder Targets](Images/All-Rounder Targets.png)

All-rounders are ranked by a combined batting + bowling impact score, rewarding players who contribute meaningfully in both departments.

**Top Targets:** Glenn Maxwell, Marcus Stoinis

---

## 🔬 Notebooks Overview

| Notebook | Purpose |
|----------|---------|
| `clean.ipynb` | Raw data cleaning — nulls, column fixes, type corrections |
| `mergingdata.ipynb` | Merges ball-by-ball + match data into unified dataset |
| `Batting_Selection.ipynb` | Batting stats, strike rate analysis, player shortlisting |
| `Bowling_Selection.ipynb` | Bowling stats, economy & wicket analysis, shortlisting |
| `All_rounders.ipynb` | Combined impact scoring for all-round players |

---

## 📌 Key Findings

| Role | Top Targets |
|------|------------|
| Opener | Jake Fraser-McGurk, Phil Salt, Jos Buttler |
| Powerplay Bowler | Trent Boult, Mohammed Shami, Arshdeep Singh |
| Death Bowler | Bhuvneshwar Kumar, Mohammed Siraj |
| All-Rounder | Glenn Maxwell, Marcus Stoinis |

---

## 🛠️ Tech Stack

- **Python 3**
- **Pandas** — data manipulation
- **NumPy** — numerical computations
- **Matplotlib / Seaborn** — visualisation
- **Jupyter Notebook** — interactive analysis

---

## 📊 Dataset

- **Source**: [IPL Dataset on Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020) 
- **Coverage**: IPL seasons up to 2024
- **Key files**: `deliveries.csv` (ball-by-ball), `matches.csv` (match results)

---

