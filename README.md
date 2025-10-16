# Investigate a Dataset: No-Show Appointments

## Project Overview

This project explores the **No-Show Appointments dataset**, which contains information about patient appointments in Brazil. The goal of this analysis is to investigate factors that might influence whether a patient shows up for their medical appointment. The analysis was conducted using **Python**, and **Pandas**, with visualizations created using **Matplotlib**.

## Research Questions
The analysis is structured around the following key questions:

1. Which neighborhoods have the poorest appointment attendance?
2. How does wait time impact appointment attendance?
3. Does having a scholarship have any impact on patient attendance?

Each question is explored through descriptive statistics, visualizations, and data summaries.

## Data Wrangling
The dataset was cleaned and prepared for analysis using Pandas. The following steps were performed:

- **Renamed columns** for readability (e.g., `No-show` → `no_show`, `AppointmentDay` → `appointment_day`).
- **Converted data types** (e.g., appointment dates to `datetime` objects, boolean conversions for categorical columns).
- **Removed invalid data** (e.g., negative ages, outliers in handicap values).
- **Created new columns** such as wait time (`appointment_day` - `scheduled_day`).

All cleaning steps are documented in the notebook.

## Exploratory Data Analysis (EDA)
Both **univariate** and **bivariate** analyses were performed:

### 1D Analysis:
- Examined distributions of individual variables such as `age`, `wait_time`, and `scholarship`.

### 2D Analysis:
- Explored relationships between variables such as:
  - `wait_time` vs. `no_show`
  - `scholarship` vs. `no_show`
  - `neighbourhood` vs. `no_show`

### Visualizations:
- Box plots  
- Bar charts

## Key Findings
- **Longer wait times** are associated with a higher likelihood of attending appointments.  
- **Scholarship recipients** are slightly less likely to attend their appointments.  
- Certain **neighborhoods** show notably higher or lower attendance rates, suggesting potential location-based influences.

## ⚖️ Limitations
- The dataset does not include **socioeconomic** or **transportation** data that might affect attendance.
- The analysis is **descriptive only**; no causal relationships are inferred.
- Additional research could include **socioeconomic** or **time-of-day patterns** approaches to narrow down the cause of poor attendance.

## 🧠 Technologies Used
- **Python 3.10+**
- **Pandas**
- **Matplotlib**
- **Jupyter Notebook**

---

## 🧩 Project Structure
Investigate_a_Dataset/
│
├── Investigate_a_Dataset.ipynb # Jupyter notebook with full analysis
├── Investigate_a_Dataset.html # HTML export for submission
├── README.md # Project documentation
└── noshowappointments.csv # Dataset file

