# Cross-Country Comparison of Hospital Length of Stay in Europe

## Overview
This project presents a **descriptive, cross-country analysis** of hospital length of stay across European countries using **official Eurostat health statistics**.

The analysis focuses on **average length of stay (ALOS)** for inpatient hospital care and examines variation between countries over time. Using aggregated, anonymised administrative data, the study explores population-level patterns in hospital utilisation rather than individual patient outcomes.

The project aims to provide insight into how health system organisation and care delivery may be associated with differences in hospital length of stay across Europe.

---

## Aim
The aims of this analysis were to:

- Compare **average hospital length of stay** across European countries  
- Examine **cross-country variation** in inpatient hospital care utilisation  
- Explore **temporal trends** in length of stay over time for selected countries  

---

## Data Source
- **Provider:** Eurostat  
- **Dataset:** `hlth_co_dischls`  
- **Indicator:** Average length of stay (ALOS)  
- **Care type:** Inpatient hospital care (ICHA-HC = HC1)  
- **Frequency:** Annual  
- **Time period:** 2010–2021  

Data were accessed in **publicly available, aggregated format**.

---

## Methods
- Retrospective **observational analysis** of aggregate Eurostat data  
- Data imported, cleaned, and processed using **Python (pandas)**  
- Analysis restricted to inpatient hospital care (HC1) and annual observations  
- Implausible values (e.g. extremely large reported lengths of stay) excluded as part of data quality checks  
- Country-level descriptive statistics calculated, including:
  - Mean length of stay  
  - Median length of stay  
- Visualisations produced using **matplotlib**

---

## Key Results

### Cross-Country Comparison of Length of Stay
A cross-country comparison demonstrated **substantial variation** in average length of stay across European countries.

Countries differed markedly in reported inpatient length of stay, reflecting heterogeneity in **health system organisation, admission practices, discharge planning, and post-acute care availability**.

---

### Countries with Shortest and Longest Stays
Countries with the shortest average lengths of stay tended to cluster around **5–6 days**, while those with longer stays exceeded **8–9 days** on average in the selected comparison year.

These differences should be interpreted cautiously, as shorter length of stay does not necessarily indicate greater efficiency or better quality of care.

---

### Trends Over Time
Trend analyses for selected countries showed a **general downward trend** in average length of stay over the study period, consistent with broader shifts towards shorter hospital admissions and expanded outpatient and community-based care.

---

## Summary Statistics
- Average length of stay varied substantially across countries  
- Most countries exhibited a gradual decline in length of stay over time  
- Cross-country differences persisted despite overall downward trends  

---

## Limitations
- Analysis based on **aggregated national data**, limiting within-country inference  
- No adjustment for **case mix, diagnosis, age structure, or comorbidity**  
- Cross-country comparisons may reflect **system-level differences** rather than clinical practice alone  
- Findings are **descriptive**, not causal  

---

## Conclusion
This analysis highlights **meaningful cross-country variation** in hospital length of stay across Europe using routinely collected Eurostat data. While overall trends suggest declining lengths of stay over time, substantial differences remain between countries.

The findings demonstrate the value of international administrative data for **comparative health systems analysis**, while underscoring the importance of cautious interpretation when detailed clinical information is unavailable.

---

## Tools Used
- Python  
- pandas  
- matplotlib  
- Jupyter Notebook  

---

## Repository Contents
- `01_download_and_clean.ipynb` — Data acquisition and cleaning  
- `02_analysis_and_figures.ipynb` — Cross-country analysis and visualisations  
- `outputs/figures/` — Saved plots  
- `outputs/tables/` — Summary tables  
