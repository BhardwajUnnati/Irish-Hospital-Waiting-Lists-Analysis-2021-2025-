#  Irish Hospital Waiting Lists Analysis (2020–2025)

##  Project Overview
This project analyzes **Irish Outpatient Waiting List data (2020–2025)** to uncover trends in hospital backlogs, waiting time bands, and patient demographics (adults vs children).  
The goal is to highlight **key problem areas** in healthcare delivery and showcase **data-driven insights** for resource allocation and policy decisions.

---

##  Dataset
- **Source:** [NTPF Ireland Open Data](https://www.ntpf.ie/waiting-list-data/open-data/)  
- **Files Used:** 2020–2025 CSVs (Outpatient Waiting Lists by Hospital)  
- **Key Attributes:**
  - `ArchiveDate` → reporting date  
  - `HospitalName` → hospital or group hospital  
  - `Adult_Child` → patient type  
  - `0-6 Months`, `6-12 Months`, `12-18 Months`, `18 Months+` → waiting time bands  
  - `Total` → total number of patients  

---

##  Tech Stack
- **Python**: Pandas, Matplotlib, Seaborn  
- **Jupyter Notebook**: EDA + Visualizations  
- **Data Cleaning**: handled missing values, removed commas, converted to datetime  
- **Visualization Tools**: Line plots, Bar charts, Heatmaps, Stacked bars  

---

##  Visualizations & Insights

### 1. Total Waiting Patients (2021–2025)
![Total Patients](images/total_patients.png)  
- Sharp rise from ~5.1M (2021) to peak ~7.4M (2022).  
- Stabilized at ~7.0M in 2023–2024.  
- Big drop in 2025 (~4.7M), but still higher than 2021.  
➡️ Backlog peaked in 2022, recovery visible by 2025.  

---

### 2. Top 10 Hospitals with Highest Waiting Patients
![Top Hospitals](images/top_hospitals.png)  
- **Galway University Hospitals** (~2.7M patients) had the highest backlog.  
- **Children’s Health Ireland, Waterford, Mater Hospital** all >2M patients.  
   Major teaching hospitals carry the heaviest burden.  

---

### 3. Patients by Waiting Time Bands (All Years)
![Waiting Bands](images/waiting_bands.png)  
- Majority of patients (~16M) wait **0–6 months**.  
- Nearly **5M patients** face extreme delays **>12 months**.  
   Long-term delays still a **systemic issue**.  

---

### 4. Adults vs Children Waiting Lists Over Time
![Adults vs Children](images/adults_vs_children.png)  
- Adults consistently make up the majority (peaking ~6.4M in 2022).  
- Children peaked ~1.05M in 2022, mirroring adult trends.  
➡️ Adults dominate waiting lists, but children follow the same crisis pattern.  

---

### 5. Heatmap: Total Patients by Hospital and Year
![Heatmap](images/hospital_heatmap.png)
- **Galway, Connolly, Cork, Waterford, Mater** stand out with highest loads.  
- Smaller hospitals show lighter shades (lower patient counts).  
   Pressure is **concentrated in a few hospitals**.  

---

### 6. Waiting Time Bands Over Years (Stacked Bar)
![Stacked Bands](images/waiting_bands_yearly.png)  
- **0–6 months** dominates across all years, peaking 2024.  
- **18 months+** backlog very high in 2021–22, improved by 2025.  
   Short-term waits are common, but **extreme delays have reduced** by 2025.  

---

## ✅ Conclusion
- Hospital waiting lists **worsened sharply from 2021 to 2022**, remained critical in 2023–24, but showed **improvement in 2025**.  
- **Galway and major teaching hospitals** (Waterford, Mater, Cork, Children’s Health Ireland) are consistently overloaded.  
- Most patients are seen within 6 months, but **millions still face delays beyond a year**.  
- Both **adults and children** experienced the same backlog trends.  

---

## 🔮 Future Work
- Add **forecasting models (ARIMA, Prophet)** for predicting 2026+ patient counts.  
- Build an **interactive Power BI / Streamlit dashboard** for real-time insights.  
- Extend analysis to **Inpatient & Day Case waiting lists** for a full picture.  

---
