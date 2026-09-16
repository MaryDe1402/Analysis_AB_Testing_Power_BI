# Analysis_AB_Testing_Power_BI
This project presents an interactive A/B Testing Analysis Dashboard designed to evaluate the impact of a product interface update. The analysis focuses on user conversion rates, engagement metrics, and user behavior (pages visited) to determine whether the changes yield statistically significant improvements.
# A/B Testing Analysis Dashboard

<img width="686" height="494" alt="image" src="https://github.com/user-attachments/assets/015495cf-f048-42d9-90f0-0b815f766fb6" />

The dashboard combines clear executive KPIs with rigorous statistical verification (**Z-test** and **Student's t-tests**), ensuring data-driven product decisions.

## 📊 Key Metrics & Visualizations
The dashboard tracks the performance of **10K total users** (split evenly: 5K Treatment / 5K Control) across three primary dimensions:
*   **Conversion (Converted):** Absolute and percentage growth in conversions.
*   **Session Duration (Average of session):** Time spent on the platform per session.
*   **Page Views (Average of pages):** The average number of pages visited by users.

All metrics are deeply broken down by **User Age Groups** (`1-25`, `25-34`, `3.35-44`, `4.45+`) to analyze segment behavior.

## 🧠 Statistical Framework & Insights

### 1. Conversion Rate (Z-Test for Proportions)
*   **Sample:** 715 conversions in `Treatment` vs 534 in `Control`.
*   **Metrics:** Z-statistic = **5.4748**, p-value = **0.00000004** ($p < 0.05$).
*   **Conclusion:** **Statistically Significant.** The Treatment variant conversion rate (14.30%) substantially outperforms the Control group (10.68%). The probability that this result occurred by chance is close to 0%.

### 2. Session Duration (Student's t-Test)
*   **Metrics:** t-statistic = **31.2500**, p-value < **0.00001** ($p < 0.05$).
*   **Conclusion:** **Statistically Significant.** The updated interface successfully holds user attention, increasing the average session duration by stable **2 minutes** (7.0 mins vs 5.0 mins).

### 3. Pages Visited (Student's t-Test)
*   **Metrics:** p-value < **0.00001** ($p < 0.05$).
*   **Conclusion:** **Statistically Significant.** Users in the Treatment group explore significantly more pages on average (**5.01 pages** vs **2.98 pages**).

## 🛠️ Tech Stack & Tools
*   **Dashboard & Visualization:** Power BI Desktop
*   **Data Processing:** Power Query & DAX formulas

