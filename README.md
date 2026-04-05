# 📊 A/B Testing Analysis: Optimization of E-commerce Conversion

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Statsmodels-3776AB?style=for-the-badge&logo=statsmodels&logoColor=white" />
  <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white" />
</p>

## 📌 Project Overview
This project evaluates the results of an A/B test conducted for an online store. The goal was to determine if specific changes in the platform (Group B) resulted in a significant increase in conversion rates and Average Order Value (AOV).

## 🛠️ Key Methodologies
* **Data Sanitization:** Removal of extreme outliers using the 99th percentile threshold.
* **Statistical Inference:**
    * **Z-Test for Proportions:** Used to validate conversion rates.
    * **Mann-Whitney U Test:** Non-parametric test used for revenue analysis due to non-normal distribution.
* **Business Intelligence:** Identification of "Data Illusions" caused by bulk corporate purchases.

## 📈 Final Insights & Decision
The analysis revealed a clear distinction between **Raw Data** and **Filtered Reality**:

| Metric | Outcome (Filtered Data) | Statistical Significance |
| :--- | :--- | :--- |
| **Conversion Rate** | **+18.86% Increase** | ✅ Significant (p < 0.05) |
| **Average Order Value** | **-3.19% Difference** | ❌ Not Significant |

### 🎯 Final Decision: **STOP THE TEST**
**Recommendation:** Implement Group B variations globally. The test proved that Group B significantly reduces friction in the user journey, increasing the volume of buyers without compromising the average spend per customer.

## 📂 Repository Structure
* `/datasets`: Contains anonymized datasets for replication.
* `notebook.ipynb`: Full Python implementation and statistical calculations.
