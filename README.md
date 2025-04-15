# Uber CSAT Drop Analysis & Monitoring Dashboard

This project dives deep into Uber's Customer Satisfaction (CSAT) trends, focusing on a noticeable decline observed in **December 2024**. It simulates how Uber’s data analytics team might investigate such drops, pinpoint causes like driver behavior or service delays, and implement an automated monitoring system using **Python, Power BI, and Airflow**.

---

## Key Findings & Actions

- **Data Sources:** Based on user reviews, ratings, and complaint data from Uber rides.
- **CSAT Drop Detected:** Between **Dec 1–20, 2024**, a sharp decline in CSAT scores was observed.
- **Root Cause Analysis:** Driver behaviour was identified as the main contributor to low scores.
- **A/B Testing:** Tested impact of the new feature (e.g., ETA transparency) — no significant CSAT difference found.
- **Dashboard:** Real-time Power BI dashboard tracks CSAT, complaint types, and A/B test results.
- **Automation:** Airflow DAG automates daily monitoring and triggers alerts on score drops or complaint spikes.

---

## Tech Stack

- **Data Analysis:** `Python`, `Pandas`, `NumPy`
- **A/B Testing:** `SciPy`, `Statsmodels`
- **Visualization:** `Power BI` (Line, Bar, Donut charts, KPIs)
- **Automation:** `Apache Airflow` (simulated with Python scripts)

---

## Process Breakdown

### 1. Data Exploration & Cleaning
- Loaded and cleaned app review dataset
- Identified complaint categories
- Extracted daily CSAT and complaint metrics

### 2. Statistical Testing
- Conducted A/B test to evaluate the effect of new features on CSAT

### 3. Dashboard Creation
- Built interactive dashboard to track:
  - CSAT trends
  - Complaint breakdowns
  - A/B group comparisons

### 4. Automated Monitoring
- Python script to check daily CSAT & complaint counts
- Simulated Airflow DAG to:
  - Monitor daily scores
  - Trigger alerts on anomalies

---

## Installation & Setup

### 1. Clone the Repository
```
git clone https://github.com/srv184/Uber_CSAT_Drop_Analysis.git
cd Uber_CSAT_Drop_Analysis
```
### 2. Install Python Dependencies
```
pip install pandas scipy statsmodels
```
### 3. Run Monitoring Script
```
python scripts/csat_monitor.py
```
### 4. (Optional) Set Up Airflow
Follow Airflow’s official guide to set up your local environment.
Once done:
Place csat_monitoring_dag.py into your Airflow DAGs folder
Start the Airflow scheduler.
### 5.Power BI Dashboard
Open the .pbix file using Power BI Desktop:
```
power_bi_dashboard/Uber_CSAT_Report.pbix
```
Use slicers to explore complaint types and A/B group performance.

---

## Conclusion

- Conducted a deep-dive analysis of customer satisfaction data.
- Identified root causes for CSAT fluctuations.
- Built an insightful and interactive dashboard.
- Developed a monitoring pipeline to catch issues early.

This project demonstrates the analytical thinking, product mindset, and technical skills required for a Data Analyst role in customer-centric platforms like Uber.
