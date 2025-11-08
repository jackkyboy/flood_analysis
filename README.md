# 🌊 Thailand Flood Analysis (2020–2023)

This repository contains an exploratory data analysis (EDA) and visualization of **Thailand's flood incidents (อุทกภัย)** from 2020 to 2023, based on open data from the Department of Disaster Prevention and Mitigation (DDPM).

---

## 📊 Overview

- **Dataset:** GD027 Flood Statistics (กรมป้องกันและบรรเทาสาธารณภัย)
- **Years Covered:** 2020–2023  
- **Events:** 10,000+ incidents normalized across 4 CSV files  
- **Goal:** Analyze flood frequency, duration, seasonality, and provincial risk pattern

---

## 🔬 Methodology

1. **Data Cleaning & Normalization**
   - Unified Thai/English column names  
   - Converted Buddhist Era → Gregorian dates  
   - Created derived metrics:  
     - `duration_days` = (end date – start date) + 1  
     - `year`, `month`  
   - Removed invalid rows (e.g. year 2111)

2. **Exploratory Analysis**
   - Yearly event trends (2020–2023)
   - Monthly seasonality histogram
   - Duration distribution
   - Provincial heatmap (Province × Year)
   - 2023 Top-20 timeline (Gantt-like)

---

## 🧩 Results Summary

| Year | Events | Mean Duration (days) | Remarks |
|------|--------:|---------------------:|---------|
| 2020 | 1,100 | 19.7 | Mild, localized floods |
| 2021 | 2,228 | 17.9 | Broader regional flooding |
| 2022 | 3,317 | 18.1 | Increasing frequency |
| 2023 | 3,697 | 47.0 | Multi-wave long duration |

### 🌦️ Seasonality
- Floods peak in **September–October** every year.  
- 2023 shows earlier onset (July–August) and prolonged duration.

### 🏙️ High-Risk Provinces (2023)
- กาฬสินธุ์ (Kalasin)
- สุโขทัย (Sukhothai)
- สกลนคร (Sakon Nakhon)
- นราธิวาส (Narathiwat)
- อุดรธานี (Udon Thani)
- นครราชสีมา (Nakhon Ratchasima)
- ร้อยเอ็ด (Roi Et)
- อุบลราชธานี (Ubon Ratchathani)
- เชียงใหม่ (Chiang Mai)

---

## 🧠 Visualization Samples

| Type | File |
|------|------|
| Yearly Trend | `charts/yearly_floods.png` |
| Monthly Histogram | `charts/monthly_floods.png` |
| Duration Distribution | `charts/duration_hist.png` |
| Province-Year Heatmap | `charts/heatmap_province_year.png` |
| 2023 Timeline | `charts/timeline_2023_top20.png` |

---

## 🧭 Repository Structure
