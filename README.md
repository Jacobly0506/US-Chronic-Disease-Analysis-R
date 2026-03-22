# 📊 US Chronic Disease Analysis: Regional Trends & Mortality
> **An R-based study on regional health disparities, obesity trends, and cardiovascular mortality using CDC data.**

[![Language](https://img.shields.io/badge/Language-R-blue.svg)](https://www.r-project.org/)
[![Library](https://img.shields.io/badge/Library-Tidyverse-orange.svg)](https://www.tidyverse.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Overview
This project leverages the **U.S. Chronic Disease Indicators (CDI)** dataset from the **CDC** to investigate the regional distribution of chronic health conditions and the correlation between behavioral risk factors (obesity, smoking) and heart disease mortality. 

By applying rigorous statistical methods in **R**, this analysis identifies critical health disparities in the U.S. South and evaluates the limitations of aggregated public health data in predicting mortality outcomes.

### 🔗 [Click Here to View the Full Analysis Report](https://jacobly0506.github.io/US-Chronic-Disease-Analysis-R/)

---

## Key Research Questions
* **Regional Disparity:** Do adult obesity rates differ significantly across U.S. Census regions (Northeast, Midwest, South, West)?
* **The "Southern" Factor:** Is the South significantly more burdened by obesity compared to the rest of the nation?
* **Correlation Analysis:** Is there a statistically significant relationship between smoking prevalence, obesity, and heart disease mortality at the state-year level?

---

## Tech Stack & Methodology

### **Core Stack**
| Category | Tools / Libraries |
| :--- | :--- |
| **Language** | R (v4.x) |
| **Libraries** | `tidyverse` (dplyr, ggplot2, tidyr), `knitr` |
| **Environment** | RStudio / R Markdown |

### **Statistical Frameworks**
* **Exploratory Data Analysis (EDA):** Visualizing distributions and identifying outliers using `ggplot2`.
* **Hypothesis Testing:** One-way **ANOVA** and **Tukey’s HSD** for regional comparisons.
* **Comparative Analysis:** **Welch Two-Sample t-test** (South vs. Others).
* **Predictive Modeling:** Simple and Multiple Linear Regression.

---

## 📈 Key Findings

### **1. Statistically Significant Regional Gap**
ANOVA results confirmed that obesity rates are not uniform across the U.S. ($p < 2 \times 10^{-16}$). Tukey’s HSD revealed the **South has significantly higher obesity rates** than the Northeast and West.

### **2. The Southern Burden**
A t-test showed the South’s mean obesity rate (**~35.7%**) is significantly higher than the combined average of the other regions (**~32.7%**).

### **3. The Aggregation Paradox**
Regression models showed a surprisingly weak correlation ($R^2 \approx 0.01$) between state-level smoking/obesity and heart disease mortality.
> **Insight:** This highlights the **Ecological Fallacy**, where state-level averages mask individual-level causalities, suggesting a need for more granular, age-adjusted data for policy intervention.
