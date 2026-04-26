# 🚗 Fuel Consumption Analysis - Phaltan, Maharashtra

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
| **Variables Collected** | 30 columns across vehicle, income, fuel, demographic data |
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
| Vehicle Type | Avg Monthly Fuel Expense (₹) |
|---|---|
| Car owners | ₹5,117 |
| Commercial vehicle | ₹9,236 |
| Bike owners | ₹4,116 |
| Scooty owners | ₹1,413 |

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
| 🔵 KPI Card 1 | Total Respondents — **569** |
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
