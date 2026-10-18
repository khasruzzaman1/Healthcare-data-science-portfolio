# Medicare Claims Analytics Portfolio — CMS DE-SynPUF

> **Medicare Claims Analytics Portfolio using CMS DE-SynPUF | MHA + MSBA (FAU 2026) | Built to demonstrate clinical analytics skills for Epic EHR implementation and population health roles at academic cancer centers**

---

## 📋 Executive Summary
This repository houses an end-to-end healthcare data science portfolio project analyzing the 2008 Centers for Medicare & Medicaid Services (CMS) Synthetic Public Use Files (DE-SynPUF). The objective is to demonstrate rigorous technical competency in Python-based healthcare data manipulation, econometric cost modeling, utilization metric tracking, and population health analytics relevant to health systems, Epic EHR deployments, and oncology research informatics.

---

## 🛠️ Technical Stack & Framework
* **Environment:** Google Colab, Python
* **Data Manipulation & Processing:** Pandas, NumPy
* **Statistical Analysis:** SciPy (`stats.ttest_ind`)
* **Data Visualization:** Matplotlib, Seaborn
* **Domain Focus:** Health Economics and Outcomes Research (HEOR), Chronic Disease Management, Value-Based Care KPIs.

---

## 🔄 6-Step Data Pipeline Architecture
1. **Load:** Securely ingested multi-gigabyte CMS beneficiary summary and inpatient claims datasets into Pandas DataFrames.
2. **Inspect:** Performed structural inspections (`.head()`, `.shape`, `.info()`) to audit data types and dimensionality.
3. **Clean:** Recoded DE-SynPUF chronic condition indicators from categorical binary codes (1/2) to true analytical flags (1/0) and computed individual `condition_count` metrics.
4. **Transform:** Engineered consolidated annual cost metrics (`total_cost`) by aggregating inpatient, outpatient, and carrier reimbursement streams.
5. **Summarize & Visualize:** Generated publication-grade portfolio visualizations:
   * *Chart 1:* Cost distributions across Medicare beneficiaries.
   * *Chart 2:* Chronic condition cost impact rankings (Highlighting cancer, diabetes, and heart failure).
   * *Chart 3:* Utilization metrics (Admissions per 1,000 members comparing diabetic vs. non-diabetic cohorts).
   * *Chart 4:* 30-day hospital readmission rate calculations (Core Epic quality metric).
6. **Validate:** Executed independent two-sample t-tests to evaluate statistical significance ($p < 0.05$) regarding chronic disease cost disparities.

---

## 📊 Key Analytical Findings
* **Population Risk Stratification:** Successfully modeled multi-morbidity burdens across beneficiaries, identifying high-cost utilization drivers.
* **Cost Disparity Validation:** Statistical hypothesis testing proved significant annual expenditure increases among high-risk chronic patient cohorts ($p < 0.001$).
* **Quality Metrics:** Computed benchmark-aligned managed care utilization rates matching standard hospital informatics frameworks.

---
*Built by Md. Khasruzzaman | Master of Health Administration & Master of Science in Business Analytics (FAU 2026)*
