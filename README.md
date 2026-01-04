# Cross-Country Comparison of Hospital Length of Stay in Europe

## Introduction
This project presents a descriptive, cross-country analysis of **hospital length of stay (LOS)** across European countries using **official Eurostat health statistics**.

Average length of stay is a commonly used indicator of hospital resource utilisation and health system organisation. Differences in LOS between countries may reflect variation in admission practices, case mix, discharge planning, availability of post-acute care, and broader health system structures.

Using aggregated, anonymised administrative data, this analysis focuses on **population-level patterns** in inpatient hospital care rather than individual patient outcomes.

---

## Data and Methods

### Data Source
- **Provider:** Eurostat  
- **Dataset:** `hlth_co_dischls`  
- **Indicator:** Average length of stay (ALOS)  
- **Care type:** Inpatient hospital care (ICHA-HC = HC1)  
- **Frequency:** Annual  
- **Time period:** 2010–2020  

The year **2010** was selected for cross-country comparison due to the best data coverage across countries.

### Methods
- Retrospective **observational analysis** of aggregated Eurostat data  
- Data imported, cleaned, and processed using **Python (pandas)**  
- Analysis restricted to inpatient hospital care (HC1)  
- Implausible values excluded as part of data quality checks  
- Descriptive statistics calculated at country level  
- Visualisations produced using **matplotlib**

---

## Results

### Cross-Country Distribution of Length of Stay (2010)
Figure 1 presents the distribution of average hospital length of stay across European countries in 2010. Substantial variation is observed, with average LOS ranging from approximately **4 to over 8 days**.

<p align="center">
  <img src="https://github.com/punarnavajha/los-europe/raw/main/outputs/figures/los_cross_country_2010.png" width="700">
</p>
<p align="center">
  <em>Figure 1. Hospital length of stay across European countries, inpatient care (HC1), 2010.</em>
</p>

---

### Countries with the Shortest Hospital Stays
Figure 2 shows the **15 countries with the shortest average hospital stays** in 2010. Turkey, Malta, and Greece exhibited the lowest reported lengths of stay, generally below **5.5 days**.

<p align="center">
  <img src="https://github.com/punarnavajha/los-europe/raw/main/outputs/figures/los_bottom15_2010.png" width="700">
</p>
<p align="center">
  <em>Figure 2. Shortest hospital stays (HC1), bottom 15 countries, 2010.</em>
</p>

---

### Countries with the Longest Hospital Stays
Figure 3 presents the **15 countries with the longest average hospital stays** in 2010. Portugal, Serbia, and Germany recorded the highest values, with average stays exceeding **8 days**.

<p align="center">
  <img src="https://github.com/punarnavajha/los-europe/raw/main/outputs/figures/los_top15_2010.png" width="700">
</p>
<p align="center">
  <em>Figure 3. Longest hospital stays (HC1), top 15 countries, 2010.</em>
</p>

---

### Trends in Length of Stay Over Time
Figure 4 illustrates trends in average hospital length of stay for selected European countries between 2010 and 2020. Most countries demonstrate a **gradual decline** over time, consistent with broader shifts towards shorter inpatient stays and increased outpatient and community-based care.

Some heterogeneity in trends remains, highlighting persistent cross-country differences.

<p align="center">
 <img src="https://github.com/punarnavajha/los-europe/raw/main/outputs/figures/los_trends_selected.png" width="750">
</p>
<p align="center">
  <em>Figure 4. Trends in hospital length of stay (HC1) for selected European countries, 2010–2020.</em>
</p>

---

## Discussion
Marked variation in hospital length of stay was observed across European countries, both in cross-sectional comparisons and over time. While overall trends suggest declining lengths of stay, substantial differences persist between health systems.

These differences likely reflect **structural and organisational factors**, including admission thresholds, discharge practices, availability of post-acute care, and population age structure. Shorter length of stay should not be interpreted as an indicator of superior quality of care without additional clinical context.

---

## Limitations
- Analysis based on **aggregated national data**, limiting within-country inference  
- No adjustment for **case mix, diagnosis, comorbidities, or age structure**  
- Cross-country comparisons may reflect **system-level reporting differences**  
- Findings are **descriptive rather than causal**

---

## Conclusion
This analysis demonstrates substantial cross-country variation in hospital length of stay across Europe using routinely collected Eurostat data. Although average lengths of stay have generally declined over time, persistent differences remain between countries.

The findings highlight the value of international administrative data for **comparative health systems analysis**, while underscoring the need for cautious interpretation when individual-level clinical detail is unavailable.

---

## Tools Used
- Python  
- pandas  
- matplotlib  
- Jupyter Notebook  

---

## Repository Contents
- `01_download_and_clean.ipynb` — Data acquisition and cleaning  
- `02_analysis_and_figures.ipynb` — Analysis and visualisations  
- `outputs/figures/` — Saved figures  
- `outputs/tables/` — Summary tables  
