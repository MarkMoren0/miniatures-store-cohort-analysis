# miniatures-store-cohort-analysis

## Miniatures Store Data Cleaning & Prep (ETL) - SalesProject.ipynb

The raw data from the miniatures store required normalization and structural changes to enable analysis. This script transforms raw transaction logs into a clean format ready for Cohort Analysis and Tableau Visualization.

Technical Stack

* Language: Python 3.x

Libraries: 

* Pandas: Data manipulation and dataframe structuring.

* NumPy: Numerical operations.

* Seaborn: Create statistical graphics to explore and understand data.

ETL Process

The script follows a structured ETL (Extract, Transform, Load) flow:

Extraction: 
* Loading raw sales data correctly (CSV format).

Transformation:

* Data Type Correction: Standardizing date formats and numeric scales.

* Purchase Status: Identifying the Days Elapsed since Last Purchase and assigning a status to each purchase.

* Loading: Exporting the cleaned dataset to a .csv for visualization.


## Data Visualization & Business Intelligence (Tableau)

The final stage of this project involves an interactive dashboard designed to translate complex data into actionable business insights. The visualization focus is on Cohort Analysis and Customer Lifetime Value (CLV).

Dashboard Architecture

* KPIs: High-level KPIs showing Number of Customers, Average Lifetime Value and Average Retention Q1.

* Cohort Heatmap: Built using a calculated field for the "Acquisition Quarter". It tracks the retention percentage of each group over subsequent periods.

* Customer Lifetime Value Growth: A visualization of cumulative revenue per cohort, identifying the Q1 2003 group as the highest-value segment over time.

* Retention Breakdown: A granular analysis showing New, Returning and Recovered customers.

* Retention Rate through Time: A longitudinal study tracking the natural decay from 56.7% to the current 17.4%, highlighting critical drop-off points in the customer lifecycle.

* Granular Data Tables: Integrated raw data views at the bottom of the dashboard to allow for "drill-down" analysis into specific transactions.

Technical Implementations

* Calculated Fields: Developed custom logic to determine the First Purchase Date per customer and calculate the Difference in Quarters between subsequent orders.

* Data Extracts (.hyper): Utilized optimized Tableau extracts to ensure high performance and seamless integration with the web-hosted version.

* Parameters & Filters: Implemented global filters to allow users to segment data by specific cohorts or timeframes.

Business Insights Derived

* High-Value Segments: Identified that the earliest cohort (Q1 2003) remains the most loyal and profitable, specifically driven by key accounts like Euro Shopping Channel and Mini Gifts Distributors Ltd.

* Stagnation Warning: The analysis revealed a halt in new customer acquisition since Q3 2004, indicating a strategic shift from growth to retention management.

* Seasonality Trends: Data confirms a consistent peak in Q4, suggesting a strong correlation with holiday-season demand, while Q1 consistently shows the lowest activity.
