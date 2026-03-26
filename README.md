# British Airways Data Science Job Simulation
**Platform:** Forage  
**Completed:** March 2026  
**Certificate:** Issued by Forage & British Airways  

---

## 📋 Overview
This repository contains my completed work for the British Airways 
Data Science Job Simulation on Forage. The simulation involved two 
independent tasks, both based on real business problems faced by 
British Airways' data and planning teams.
A certificate of completion was issued by Forage on March 25th, 2026.

---

## ✈️ Task 1: Lounge Eligibility Modelling (Heathrow Terminal 3)

### Problem
British Airways needed a flexible, reusable model to forecast how 
many passengers would be eligible for each of its 3 premium lounges 
at Heathrow Terminal 3, without knowing exact future flight schedules.

### My Approach
- Analysed a 10,000 flight BA summer schedule dataset
- Grouped flights by haul type (Long-Haul / Short-Haul / Domestic) 
  and time of day (Morning / Lunchtime / Afternoon / Evening)
- Derived eligibility percentages for each lounge tier directly 
  from the data using average eligible passengers ÷ total seats
- Delivered a reusable Excel lookup table, planners input total 
  passengers and eligibility figures calculate automatically

### Lounge Tiers Modelled
| Tier | Lounge | Who Qualifies |
|------|--------|---------------|
| 1 | Concorde Room | First Class + Gold Guest List members |
| 2 | First Lounge | BA Gold Executive Club members |
| 3 | Club Lounge | Club World (Business) + BA Silver members |

### Key Finding
Short-haul routes show significantly higher lounge eligibility 
percentages (16-17% Tier 3) compared to long-haul routes (10-11%), 
driven by the higher concentration of frequent business flyers 
on European routes.

### Files
- `British Airways Summer Schedule Dataset - Forage Data Science Task 1.xlsx` - Dataset
- `Lounge Eligibility Lookup and Justification - Task 1.xlsx` -
   lookup table + written justification

---

## 🤖 Task 2: Customer Booking Completion Prediction

### Problem
Only 15% of customers who begin a booking actually complete it. 
British Airways wanted to understand which factors drive a customer 
to complete their booking, so the marketing team can proactively 
target high-intent customers before they book with a competitor.

### My Approach
- Trained a **Random Forest classifier** (200 trees, balanced class 
  weights) on 50,000 customer booking records
- Engineered 5 new features from existing columns
- Evaluated using ROC-AUC and 5-fold cross-validation
- Handled class imbalance (85/15 split) using `class_weight='balanced'`

### Results
| Metric | Value |
|--------|-------|
| ROC-AUC (Test Set) | **75.9%** |
| ROC-AUC (5-Fold CV) | **75.0% ± 0.005** |
| Recall - Bookings Found | **70.3%** |
| Overall Accuracy | **69.6%** |

### Top 5 Predictors of Booking Completion
| Rank | Feature | Importance |
|------|---------|------------|
| 1 | Booking Origin (country) | 40.1% |
| 2 | Length of Stay | 10.5% |
| 3 | Flight Duration | 10.4% |
| 4 | Purchase Lead Time | 9.1% |
| 5 | Flight Hour | 5.9% |

### Key Insight
Where a customer books from accounts for **40% of the model's 
predictive power**, suggesting BA needs country-specific 
re-engagement strategies rather than a single global campaign.

### Files
- `BA_Task2_CustomerBookingPrediction.ipynb` - Full Python notebook 
   with code, outputs and charts
- `customer_booking.csv` - Dataset (50,000 records, 14 features)

---

## 🛠️ Tools & Technologies
- **Python** - pandas, scikit-learn, matplotlib, numpy
- **Machine Learning** - Random Forest, cross-validation, 
  feature engineering
- **Excel** - openpyxl, formula-driven models
- **Reporting** — Excel lookup models, written justification

---

## 📜 Certificate
**Nayana Agrahara Dattatri**  
British Airways Data Science Job Simulation  
Issued by Forage - March 25th, 2026  
Enrolment Verification Code: `yrLfF9w9QNBdBvsfH`

---
## 🔗 Connect
[LinkedIn]([https://linkedin.com/in/your-profile](https://www.linkedin.com/in/nayana-agrahara-dattatri-06761614a/))
