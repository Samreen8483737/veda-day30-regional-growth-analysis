# Day 30: Regional Growth Analysis

## Objective
Execute period-over-period comparisons to evaluate regional sales performance, identify true revenue drivers, and isolate statistical distortions such as the small-base effect.

## Technical Implementation
* **SQL:** Utilized the `LAG()` window function to align previous and current period sales onto a single row, enabling accurate absolute variance and percentage growth calculations.
* **Data Visualization (Google Sheets):** Engineered a Combo Chart utilizing a secondary Y-axis to simultaneously map Absolute Growth (clustered columns) and Growth Rate Percentage (line). This dual-axis approach visually separated raw revenue impact from relative percentage spikes.

## Key Insights & Business Value
1. **The Small-Base Effect:** The South region exhibited an explosive 500% growth rate. However, because the previous period baseline was only $1,000, this massive percentage merely represented a $5,000 actual revenue increase, demonstrating how isolated percentages can severely mislead executive strategy.
2. **True Volume Driver:** The North region generated the highest absolute revenue growth ($15,000). Despite displaying a much lower relative growth rate of 15%, this territory provided the most tangible bottom-line value to the business.
3. **Contraction Alert:** The East region experienced a 3.53% contraction, representing a $3,000 drop in revenue. This negative variance requires immediate operational review to identify the root cause.
4. **Metric Pairing:** The analysis proves that evaluating regional performance requires pairing percentage growth with absolute dollar growth to prevent resource misallocation toward artificially inflated metrics.
