# Excel_Project
India CPI Inflation Analysis

# Executive Summary
This financial modeling project evaluates historical Consumer Price Index (CPI) trends in India (2013–2023) and measures the pass-through impact of global crude oil prices on domestic inflation categories. Using official dataset from the Ministry of Statistics and Programme Implementation (MOSPI) and crude oil FOB pricing, this workbook analyzes rural vs. urban spending differences, tracks MoM food inflation, and calculates correlation metrics across major consumption buckets.

# Dataset Architecture & Methodology
The analysis spans 7 integrated modules:
1. **Historical Baseline (`All_India_Index`):** Cleaned monthly CPI readings across Rural, Urban, and Combined sectors across 25+ commodity categories.
2. **Basket Weighting Analysis (`PROBLEM 1`):** Category distribution modeling highlighting rural vs. urban consumption weight disparities.
3. **Annual YoY Inflation Tracker (`PROBLEM 2`):** Automated pivot-based YoY inflation modeling using `GETPIVOTDATA`.
4. **MoM Food Dynamics (`PROBLEM 3`):** High-frequency monthly inflation tracking across food & beverage sub-components (May 2022 – May 2023).
5. **Macro Category Indexing (`PROBLEM 4`):** Aggregation of 20+ line items into macro economic indicators (Essentials, Health, Food, Energy).
6. **Crude Oil Pass-Through Analysis (`PROBLEM 5`):** Pearson correlation matrix evaluating inflation sensitivity against Indian Basket Crude Oil FOB prices.

# Key Findings & Strategic Insights

### 1. Rural vs. Urban Expenditure Asymmetry
- **Food Dominance:** Food & Beverages account for ~48.9% of total expenditure allocation in rural areas compared to ~48.5% in urban areas.
- **Housing Impact:** Urban CPI inflation is heavily influenced by housing indices (~7.2% allocation), which are absent from the rural CPI calculation basket.

### 2. Crude Oil Price Sensitivity (Pass-Through Analysis)
Statistical correlation (`CORREL`) against the Indian Basket Crude Oil Price Index revealed varying levels of sensitivity across components:
- **High Positive Correlation:** Oils & Fats ($r \approx 0.81 - 0.83$), Meat & Fish ($r \approx 0.76$), and Transport & Communication ($r \approx 0.65 - 0.68$).
- **Moderate Positive Correlation:** Fuel & Light ($r \approx 0.56 - 0.58$) and Spices ($r \approx 0.55 - 0.60$).
- **Negligible / Inverse Correlation:** Egg prices exhibited a negative correlation ($r \approx -0.17 \text{ to } -0.23$), reflecting supply-driven domestic seasonality rather than import parity pricing.
