# 📊 Marketing Science Case Study: Lead Optimization

**Candidate:** Juan  
**Objective:** Analyze a 2nd-year automotive dataset to identify lead generation opportunities, evaluate the ICE-to-BEV market transition, and forecast 2025 performance.

---

## 🛠️ Technical Pipeline & Data Integrity (Q4)

Before performing the analysis, a rigorous **ETL (Extract, Transform, Load)** process was implemented to ensure the scientific validity of the results:

- **Automated Conversion:** Developed a Python routine to batch-convert raw Excel sheets into standardized CSV files[cite: 65, 66, 68].
- **Data Audit & Cleaning:** \* Identified and resolved a **temporal data leak** where 2024 records were discovered within the 2023 source file[cite: 74].
  - Standardized disparate headers (e.g., aligning `showrooms_visits` to `car_model_visits`) to ensure year-over-year parity[cite: 72].
  - Implemented a `clean_columns` function to handle whitespace and naming conventions programmatically[cite: 70, 71].
- **Feature Engineering:** Engineered a unified `total_leads` metric by aggregating specific high-intent actions: **Test Drives**, **Finance Leads**, and **Quote Requests**[cite: 83].

---

## 📈 Key Analytical Findings

### 1. Popularity & Momentum (Q1)

- **The Volume Leader:** Models were ranked based on absolute visits and **Configuration Completion Rate (CCR)** to distinguish between "Browsers" and "Buyers"[cite: 76].
- **Strategic Insight:** Volume alone does not dictate value; the analysis focuses on intent-driven metrics to prioritize marketing spend[cite: 75].

### 2. Efficiency Gaps & "Margin for Improvement" (Q2)

- **The Funnel Bottleneck:** Performed a deep-dive into the configurator journey for **Models B, C, and E**[cite: 80].
- **Findings:** The primary "Margin for Improvement" was identified at the **'Start Configuration'** stage rather than completion[cite: 81, 82]. Users are showing interest (visits) but are not entering the tool, suggesting a Call-to-Action (CTA) or landing page friction[cite: 78].
- **Benchmark:** Model_C serves as the operational benchmark for high-efficiency funnel performance[cite: 80].

### 3. The Electric Shift: ICE vs BEV (Q3)

- **The BEV Paradox:** While overall traffic (visits) showed a slight contraction for Electric models, **Lead volume increased by ~94% YoY**[cite: 85, 87].
- **The Takeaway:** The brand is successfully transitioning from an "Awareness" phase to a "High-Intent" phase in the electric segment[cite: 83].

---

## 🤖 Statistical Modeling & Predictive Analytics

To move beyond descriptive statistics, the following models were implemented:

- **Linear Regression (2025 Forecast):** Projected lead volume into the next fiscal year based on monthly growth trends, estimating a significant increase in total lead output for 2025[cite: 95].
- **Random Forest (Driver Analysis):** Utilized a machine learning approach to rank feature importance.
  - **Top Driver:** `Complete Configuration` was identified as the strongest predictor of a final lead[cite: 96].
  - **Insight:** Validates the business focus on driving users through the full configuration journey.
- **Seasonality Analysis:** Identified "Peak Performance" months and days of the week, allowing for the optimization of marketing "Flighting" (budget scheduling)[cite: 93, 94].

---

## 💡 Strategic Recommendations

1.  **Scale Model_E:** Identified as a "Hidden Gem" with a high Lead Conversion Rate (LCR) but low volume; shifting budget here maximizes ROI[cite: 89].
2.  **Fix the BEV Start-Funnel:** Address the 2024 "Start Rate" drop-off to capture the high intent seen in the Electric segment[cite: 91, 92].
3.  **Front-load Weekday Spend:** Based on daily averages, marketing spend should be optimized for Monday–Thursday when conversion intent peaks[cite: 93].

---

> **Note on Visualization:** All charts utilize a custom-branded color palette (`#0d47c7` Blue and `#f24819` Orange) on a neutral background (`#f6faf3`) for a professional, client-ready aesthetic[cite: 85, 94].

---
