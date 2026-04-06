# Replication: "The Morale Effects of Pay Inequality"
### Breza, Kaur & Shamdasani (2016), NBER Working Paper No. 22491

---

## Overview
This repository contains replication code and output for:

> Breza, E., Kaur, S., & Shamdasani, Y. (2016). *The Morale Effects 
> of Pay Inequality*. NBER Working Paper No. 22491.

The paper uses a **randomized field experiment** with 378 manufacturing 
workers in Odisha, India to test whether workers care about pay relative 
to co-workers, and whether perceived justifications mediate fairness concerns.

---

## Experiment Design
- **378 workers** across 14 one-month rounds, 3 factory sites
- Workers organized into **units of 3**, randomized into 4 wage treatments:
  - Pay Disparity (wLow, wMed, wHigh by rank)
  - Compressed Low (all paid wLow)
  - Compressed Medium (all paid wMed)
  - Compressed High (all paid wHigh)
- **Outcome variables:** Daily output (standardized), attendance
- **Key identification:** DiD comparing same-wage workers across 
  Pay Disparity vs Compressed units

---

## Data
Data is publicly available from the AEA dataverse:
🔗 [Download Data Here](https://www.openicpsr.org/openicpsr/project/113593)

Download these files and place them in the root directory:
- `finaldataset.dta` — Main panel dataset (worker × day)
- `el_games1.dta` — Endline tower building game
- `el_games2.dta` — Endline cooperative puzzle games

---

## Requirements
- **Stata 14 or higher** (replicated using Stata 17)
- **estout** package for table formatting

Install estout if needed:
```stata
ssc install estout
```

---

## How to Run

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/pay-inequality-replication.git
```

2. Download data from AEA dataverse and place `.dta` files in root folder

3. Open `code/replication_code_main.do` in Stata

4. Update the global path at the top:
```stata
global dir "YOUR_PATH_HERE"
global date "2024"
```

5. Run the do-file:
```stata
do "code/replication_code_main.do"
```

---

## Tables Replicated

| Table | Description | Status |
|-------|-------------|--------|
| Table 2 | Summary Statistics | ✅ Replicated |
| Table 3 | Knowledge of Co-worker Wages | ✅ Replicated |
| Table 4 | Main Effects of Pay Disparity | ✅ Replicated |
| Table 5 | Effects Over Time | ✅ Replicated |
| Table 6 | Perceived Justifications | ✅ Replicated |
| Table 7 | Unit Level Variation | ✅ Replicated |
| Table 8 | Endline Games 1 (Tower Building) | ✅ Replicated |
| Table 9 | Endline Games 2 (Cooperative Puzzles) | ✅ Replicated |
| Table 10 | Network Formation | ✅ Replicated |
| Table 11 | Fairness and Happiness | ✅ Replicated |

---

## Figures Replicated

| Figure | Description | Status |
|--------|-------------|--------|
| Figure 4 | Effects of Pay Disparity on Worker Output | ✅ Replicated |
| Appendix Figure 2 | Attendance Distribution | ✅ Replicated |
| Appendix Figure 5 | Village Wage Distribution | ✅ Replicated |

---

## Key Findings Verified

- Pay disparity reduces output by **0.242 SD** (Table 4, Col 2)
- Pay disparity reduces attendance by **11.7 pp** (Table 4, Col 4)
- Effects strengthen over time — largest after second payday (Table 5)
- Effects disappear when productivity differences are large or 
  output is easily observable (Table 6)
- Pay disparity units build towers **17% shorter** in endline games (Table 8)
- Pay disparity workers perform **28% worse** with own unit members 
  vs strangers in puzzle games (Table 9)

---

## Discrepancies Found
*(To be updated after full replication)*

---

## Replicator
**Ravi S**  
Replication completed: April 2026  
Contact: [your email]
