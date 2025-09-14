# Industrial-Machine-downtime--Analysis

## Objective
To diagnose and quantify the primary drivers of operational inefficiency by analyzing historical machine downtime data. The core goal is to move beyond reactive problem-solving by developing a diagnostic framework that identifies predictive indicators of machine failure. This analysis will culminate in a strategic recommendation for a preventative maintenance program, designed to increase Overall Equipment Effectiveness (OEE) and reduce costs.

---

## Data Cleaning & Preparation
The initial dataset contained several data quality issues, including missing values, inconsistent text formatting, incorrect data types, and outliers. A rigorous cleaning process was performed which included:
* Standardizing categorical text (`Reason_Code`).
* Converting numerical columns to their correct data types and handling text errors.
* Visualizing outliers using box plots and flagging them for imputation.
* Imputing missing numerical values using the median to ensure robustness.

---

## Key Findings & Visualizations

### 1. 'Mechanical' Failures are the Primary Cause of Downtime
The analysis revealed that mechanical failures are overwhelmingly the largest source of lost production hours.

<img width="1306" height="546" alt="Chart1" src="https://github.com/user-attachments/assets/87280218-5ffd-41a3-9e24-104594bafbaf" />

### 2. Lack of Maintenance is a Key Predictor of Failure
A strong correlation was found between the number of days since the last maintenance and the occurrence of severe mechanical failures, with a sharp increase in risk after 90 days.

<img width="1015" height="639" alt="Chart2" src="https://github.com/user-attachments/assets/e3377fba-da7d-4722-9310-ae95d4a8d275" />

### 3. Night Shift Shows Higher Operator Error Rates
The 'Night' shift accounts for a disproportionately high percentage of operator errors, suggesting a potential issue with training or procedures.

<img width="1004" height="638" alt="chart3" src="https://github.com/user-attachments/assets/db5574e0-6bfd-4d7c-abec-1732c2a5a8a3" />

---

## Actionable Recommendations

1.  **Implement a 90-Day Preventative Maintenance Cycle:** Mandate a preventative maintenance schedule for all critical machinery at a maximum 90-day interval to proactively address the primary cause of production loss.
2.  **Conduct a Night Shift Process & Training Review:** Initiate a review of night shift procedures and training protocols to reduce the high rate of operator errors.
3.  **Prioritize an Audit of Machine HMC-03:** Conduct a full diagnostic audit of the least reliable machine, HMC-03, to identify and rectify its underlying issues.
