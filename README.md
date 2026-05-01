# 🚗 Fuel Consumption Analysis — Phaltan, Maharashtra

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Statistics](https://img.shields.io/badge/Statistics-Regression%20%7C%20ANOVA%20%7C%20Correlation-blue?style=for-the-badge)
![Survey](https://img.shields.io/badge/Survey-567_Respondents-orange?style=for-the-badge)
![Location](https://img.shields.io/badge/Location-Phaltan%2C_Maharashtra-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

> **A comprehensive statistical analysis of monthly household fuel consumption patterns across 567 households in Phaltan, Maharashtra — using primary survey data, multiple regression, ANOVA, hypothesis testing, and an interactive Excel dashboard.**

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Key Findings](#-key-findings)
- [Dashboard Preview](#-dashboard-preview)
- [Objectives](#-objectives)
- [Methodology](#-methodology)
- [Statistical Results](#-statistical-results)
- [Tools Used](#-tools-used)
- [Dataset](#-dataset)
- [File Structure](#-file-structure)
- [How to Open](#-how-to-open)
- [Skills Demonstrated](#-skills-demonstrated)

---

## 📌 Project Overview

This project examines **monthly fuel consumption behaviour** of households in Phaltan, a city in Satara district, Maharashtra. The study was conducted as a primary survey covering **567 households**, collecting data on vehicle ownership, income levels, fuel expenditure, family size, and commute distance.

The analysis identifies the key **drivers of fuel consumption**, estimates **per capita fuel expenditure**, and provides **data-backed recommendations** for sustainable transport planning in Phaltan.

| Detail | Value |
|--------|-------|
| **Location** | Phaltan, Satara District, Maharashtra |
| **Survey Period** | October 2025 |
| **Sample Size** | 567 households |
| **Original Responses** | 597 (30 removed during cleaning) |
| **Variables Collected** | 30 columns after cleaning (original: 41) |
| **Analysis Method** | Descriptive Statistics, Regression, ANOVA, Hypothesis Testing |
| **Tool** | Microsoft Excel (with Analysis ToolPak) |

---

## 🔑 Key Findings

### 1. Per Capita Fuel Expenditure
| Metric | Value |
|--------|-------|
| **Average monthly per capita fuel expense** | ₹750 / person / month |
| Median per capita | ₹400 / person / month |
| Minimum | ₹40 / person / month |
| Maximum | ₹5,000 / person / month |
| Standard Deviation | ₹763 |

> The right-skewed distribution (mean > median) indicates that a small number of high-income, multi-vehicle households significantly pull the average upward.

---

### 2. Fuel by Vehicle Type
| Vehicle Type | Avg Monthly Fuel (Litres) | Avg Monthly Fuel Expense (₹) |
|---|---|---|
| Commercial vehicle owners | 69.10 L | ₹9,236 |
| Car owners | 27.20 L | ₹5,117 |
| Bike owners | 10.50 L | ₹4,116 |
| Scooty owners | 7.14 L | ₹1,413 |

---

### 3. Fuel by Income Group
| Income Group | Avg Per Capita Fuel (₹) | Count |
|---|---|---|
| Below ₹10,000 | 319 | 125 |
| ₹10,000 – 30,000 | 419 | 101 |
| ₹30,000 – 50,000 | 804 | 203 |
| ₹50,000 – 70,000 | 1,075 | 98 |
| ₹70,000 – 1,00,000 | 1,447 | 23 |
| Above ₹1,00,000 | 2,429 | 17 |

---

### 4. Fuel by Vehicle Ownership
| Vehicles Owned | Avg Monthly Fuel Expense (₹) | Count |
|---|---|---|
| 1 vehicle | 1,657 | 357 |
| 2 vehicles | 5,574 | 171 |
| 3 vehicles | 8,729 | 38 |
| 4 vehicles | 15,000 | 1 |

---

### 5. Regression — What Drives Fuel Consumption?

> Multiple regression using 4 predictors explains **51.76%** of the variation in monthly fuel expenditure — nearly double the explanatory power of income alone.

**Regression Equation:**
```
Fuel Expense = −4,215 + 0.034(Income) + 2,716(Num_Vehicles) + 375(Family_Members) + 88(Distance)
```

| Predictor | Coefficient (β) | p-value | Significance |
|---|---|---|---|
| **Number of Vehicles** | +2,716 | 9.84 × 10⁻³⁸ | ✅ Highly significant |
| **Monthly Income** | +0.034 | 6.97 × 10⁻¹³ | ✅ Significant |
| **Family Members** | +375 | 0.00057 | ✅ Significant |
| **Home–Work Distance (km)** | +88 | 0.000152 | ✅ Significant |

**Interpretation:** Every additional vehicle a household owns adds ₹2,716 to their monthly fuel bill. Every extra km of commute adds ₹88/month.

---

## 📊 Dashboard Preview

The project includes an **interactive Excel dashboard** featuring:

| Element | Description |
|---|---|
| 🔵 KPI Card 1 | Total Respondents — **567** |
| 🟢 KPI Card 2 | Average Monthly Fuel Expense |
| 🟠 KPI Card 3 | Average Per Capita Fuel — **₹750/month** |
| 🟣 KPI Card 4 | Income–Fuel Correlation — **r = 0.518** |
| 📊 Chart 1 | Avg Fuel Expense by Vehicle Type (Bar chart) |
| 📊 Chart 2 | Avg Fuel Expense by Income Group (Column chart) |
| 📊 Chart 3 | Avg Fuel Expense by Num Vehicles (Column chart) |
| 📊 Chart 4 | Per Capita Fuel Distribution (Histogram) |
| 🎛️ Slicer 1 | Filter by **Gender** |
| 🎛️ Slicer 2 | Filter by **Income Group** |

> All PivotCharts respond to slicers — clicking "Female" or an income group instantly filters all 4 charts simultaneously.

---

## 🎯 Objectives

| # | Objective | Status |
|---|---|---|
| O1 | Estimate average monthly fuel consumption by vehicle type | ✅ Complete |
| O2 | Estimate monthly per capita fuel consumption in Phaltan | ✅ Complete |
| O3 | Study the relationship between income and fuel consumption | ✅ Complete |
| O4 | Examine the effect of vehicle ownership on fuel consumption | ✅ Complete |
| O5 | Test statistical significance using appropriate hypothesis tests | ✅ Complete |
| O6 | Suggest sustainable transport planning strategies | ✅ Complete |
| O7 | Examine factors affecting fuel consumption (regression) | ✅ Complete |

---

## 🔬 Methodology

### Data Collection
- **Method:** Primary survey (Google Form)
- **Sampling:** Households across Phaltan city
- **Variables:** Vehicle types, fuel expenses per vehicle, income bracket, family size, commute distance, gender, EV interest, public transport usage

### Data Cleaning (Excel)
- Removed 30 invalid/duplicate rows (597 → 567)
- Renamed all 30 columns to clean `snake_case` format
- Extracted numeric values from text (e.g. `"15 L"` → `15`, `"₹6,500"` → `6500`)
- Standardised 15 occupation variants → 9 clean categories
- Fixed misplaced data in wrong columns (PT_Frequency had vehicle names; Vehicle_Purpose had frequency values)
- Replaced junk values with blank (NaN) in numeric columns
- Filled missing numeric values with **median** (vehicle-specific blanks left as-is — blank = "no vehicle")
- Created helper columns in dedicated analysis sheets: `Has_Bike`, `Has_Scooty`, `Has_Car` (in `Fuel_Data_Used_Avg_Fuel(l)`) and `Income_Numeric` (in `Correlation`), `Per_Capita_Fuel` (in `Per_Capita_Expenses`)

### Analysis Pipeline
```
Raw Survey Data (597 rows)
        ↓
Data Cleaning & Validation (567 rows, 30 cols)
        ↓
Descriptive Statistics + PivotTables
        ↓
Correlation Analysis (r = 0.518)
        ↓
ANOVA — Vehicle Type & Ownership Effect
        ↓
Hypothesis Testing (T-test, ANOVA ×2, Correlation)
        ↓
Multiple Linear Regression (4 predictors)
        ↓
Interactive Excel Dashboard
        ↓
Recommendations & Report
```

---

## 📐 Statistical Results

### Hypothesis Tests Summary

| Test | H₀ | p-value | Decision |
|---|---|---|---|
| **H1 — T-test** | No gender difference in fuel spending | **t = 12.86, p = 5.27 × 10⁻³⁰** | ✅ Reject H₀ |
| **H2 — ANOVA** | No difference across income groups | **F = 41.79, p = 1.39 × 10⁻³⁶** | ✅ Reject H₀ |
| **H3 — ANOVA** | Vehicle ownership has no effect | **9.98 × 10⁻⁷²** | ✅ Reject H₀ |
| **H4 — Correlation** | No correlation between income and fuel | **p < 0.05** (r=0.518) | ✅ Reject H₀ |

### ANOVA — Vehicle Ownership Effect
```
F(3, 563) = 150.81    p = 9.98 × 10⁻⁷²    α = 0.05
```
> The most statistically significant finding in the study. Vehicle ownership explains **44.56% of fuel expenditure variance** (η² = 0.4456 — large effect size).

### Multiple Regression Summary
```
Adjusted R²     = 0.5176   (51.76% variance explained)
F-statistic     = 152.82
Significance F  = 2.21 × 10⁻⁸⁸
Observations    = 567
Standard Error  = ₹2,436
```

### Correlation
```
Income vs Total Fuel Expense:  r = 0.518  (Moderate positive)
```

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Primary analysis tool |
| **Excel PivotTables** | Group-level summaries and cross-tabulations |
| **Excel PivotCharts** | Interactive dashboard charts |
| **Analysis ToolPak** | Regression, ANOVA, Correlation, Histogram |
| **Excel Slicers** | Dashboard interactivity (filter by gender/income) |
| **Conditional Formatting** | Data quality checks (highlighting blanks, outliers) |
| **AVERAGEIF / COUNTIF** | Group-wise calculations |
| **T.TEST formula** | Gender hypothesis test |
| **CORREL formula** | Pearson correlation coefficient |
| **Nested IF formulas** | Income numeric conversion, vehicle dummy variables |

---

## 📁 Dataset

| Variable | Type | Description |
|---|---|---|
| `Total_Monthly_Fuel_Expense` | Numeric | Household total fuel spend (₹/month) |
| `Per_Capita_Fuel` | Numeric (derived) | Expense ÷ family members |
| `Income_Numeric` | Numeric (derived) | Income bracket midpoint (₹) |
| `Num_Vehicles` | Integer | Total vehicles in household |
| `Family_Members` | Integer | Number of people in household |
| `Home_Work_Distance_km` | Numeric | Daily commute distance (km) |
| `Monthly_Income` | Category | 6 income brackets |
| `Gender` | Category | Male / Female / Prefer not to say |
| `Vehicle_Types` | Category | Combined vehicle ownership types |
| `Has_Bike / Has_Car / Has_Scooty` | Binary (derived) | Vehicle type dummy variables |
| `Consider_EV` | Category | Yes / No / Maybe |
| `PT_Frequency` | Category | Public transport usage frequency |

---

## 📂 File Structure

```
fuel-consumption-phaltan/
│
├── 📊 Fuel_Consumption_Analysis_project.xlsx     ← Main analysis workbook (26 sheets)
│   │
│   ├── [RAW & CLEAN DATA]
│   │   ├── Form Responses 1              ← Original 597 raw survey responses
│   │   └── clean_data                    ← Cleaned dataset (567 rows × 30 columns)
│   │
│   ├── [DESCRIPTIVE ANALYSIS]
│   │   ├── Clean_Data_Summary            ← Summary statistics table
│   │   ├── Descriptive_Statistics        ← Mean, median, SD, skewness per variable
│   │   ├── Outlier_detection             ← IQR method outlier identification
│   │   ├── Pie_Chart                     ← Vehicle type ownership distribution
│   │   └── Box_plot                      ← Distribution by group
│   │
│   ├── [OBJECTIVE 1 — Avg fuel by vehicle type]
│   │   ├── Fuel_Data_Used_Avg_Fuel(l)    ← Helper columns: Has_Bike, Has_Car, Has_Scooty
│   │   ├── Avg_Fuel(LMonth)              ← Avg litres per vehicle type
│   │   └── Avg_Fuel_Expense              ← Avg ₹ expense per vehicle type
│   │
│   ├── [OBJECTIVE 2 — Per capita fuel]
│   │   ├── Per_Capita_Expenses           ← Per_Capita_Fuel column + summary stats
│   │   ├── Histrogram                    ← Per capita distribution histogram
│   │   └── per_capita_fuel               ← Per capita regression analysis
│   │
│   ├── [OBJECTIVE 3 — Income vs fuel]
│   │   ├── Correlation                   ← Income_Numeric + CORREL results
│   │   └── Correlation_Matrix            ← Full variable correlation matrix
│   │
│   ├── [OBJECTIVE 4 & 5 — Vehicle ownership + Hypothesis tests]
│   │   ├── ANOVA1                        ← ANOVA: vehicle ownership effect
│   │   ├── ANOVA2                        ← ANOVA: income groups
│   │   ├── T-test                        ← T-test: gender vs fuel spending
│   │   └── Hypothesis_Summary            ← All 4 tests summary table
│   │
│   ├── [OBJECTIVE 7 — Regression]
│   │   ├── Regression1                   ← Multiple regression (expense as Y)
│   │   └── Regression2                   ← Regression (per capita as Y)
│   │
│   ├── [OUTPUT & RECOMMENDATIONS]
│   │   ├── Recomendations                ← Sustainable transport strategies
│   │   ├── Project_Summary               ← Summary of all findings
│   │   ├── Pivot_Charts                  ← PivotTable data for dashboard
│   │   └── Dashboard                     ← Interactive Excel dashboard with slicers
│
├── 📄 Project_Summary_Report.docx        ← Project summary report (editable Word)
├── 🖼️ Dashboard_AllData.png              ← Dashboard screenshot (all data)
├── 🖼️ Dashboard_Female.png               ← Dashboard filtered by Female
├── 🖼️ Dashboard_HighIncome.png           ← Dashboard filtered by high income
└── 📖 README.md                          ← This file
```

---

## 📂 How to Open

1. **Download** `Fuel_Consumption_CLEAN.xlsx`
2. Open in **Microsoft Excel 2013 or later**
3. If prompted, click **Enable Content** to allow macros/PivotTables to refresh
4. Navigate to the **Dashboard** sheet (last tab, coloured dark blue)
5. Click any button in the **Gender** or **Income Group** slicer to filter all charts

> **Note:** The Analysis ToolPak add-in was used for regression and ANOVA. To re-run these analyses: File → Options → Add-ins → Excel Add-ins → tick Analysis ToolPak.

---

## 💼 Skills Demonstrated

```
Data Analysis          ████████████████████  Advanced
Statistical Testing    ███████████████████░  Advanced
Data Cleaning          ████████████████████  Advanced
Data Visualisation     ██████████████████░░  Advanced
Excel (PivotTables)    ████████████████████  Advanced
Regression Modelling   █████████████████░░░  Intermediate–Advanced
Dashboard Design       ████████████████░░░░  Intermediate
Report Writing         ████████████████████  Advanced
```

**Technical skills used in this project:**
`Microsoft Excel` · `Descriptive Statistics` · `Hypothesis Testing` · `Pearson Correlation` · `Multiple Linear Regression` · `One-way ANOVA` · `T-test` · `PivotTables` · `PivotCharts` · `Dashboard Design` · `Data Cleaning` · `Survey Research` · `Data Visualisation` · `Report Writing`

---

## 🌱 Sustainable Transport Recommendations

Based on the analysis findings:

1. **Vehicle-sharing initiatives** — Vehicle ownership is the strongest fuel consumption driver (β=2,716). Promoting carpooling and shared mobility in Phaltan can significantly reduce per-household fuel burden.
2. **Electric 2-wheeler subsidies** — Targeting students and agricultural workers (the two largest respondent groups) with EV subsidy schemes to reduce petrol dependency.
3. **Improved public transport** — Home-to-work distance significantly predicts fuel use (β=88/km). Better bus/auto-rickshaw connectivity on high-commute corridors reduces personal vehicle dependency.
4. **Tiered fuel policy** — High-income households (above ₹1 lakh) spend 7.6× more per capita than low-income households. A tiered approach to fuel taxation with cross-subsidisation for lower-income groups can improve equity.
5. **EV charging infrastructure** — Survey data shows a meaningful proportion of respondents are open to EV adoption — infrastructure investment in Phaltan will accelerate this transition.

---

## 👤 Author

**Aditi Subhash Jadhav**
Statistics Student | Data Analysis Enthusiast

📧 aditijadhav416@gmail.com
🔗 (https://www.linkedin.com/in/aditi-jadhav-3b2310385)
📍 Phaltan, Maharashtra, India

---

*This project was completed as part of a research/academic project in 2025–26.*
