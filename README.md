# AB-Test-Conservation-Campaign
Analysis of A/B testing data for a conservation campaign's personalized vs. generic messaging, visualized in Power BI.
# Conservation Campaign: A/B Test Results Dashboard

## Project Objective
This project analyzes the results of an A/B test conducted for a conservation campaign. The primary objective was to determine whether personalized messaging led to a statistically significant increase in user engagement compared to generic messaging, and to quantify the impact.

## Dashboard Screenshot
![Screenshot 2025-06-01 230125](https://github.com/user-attachments/assets/e945d8a0-4ff2-43b9-b3af-69c4cd69e191)


## Key Findings & Visualizations
The Power BI dashboard presents the following key insights:
* **Conversion Rates:** Displays the engagement rates for both the 'Personalized' and 'Generic' message groups.
* **Uplift:** Highlights the percentage increase in engagement achieved by the personalized messaging.
* **Statistical Significance:** Shows the P-value from the Chi-Squared test, confirming the reliability of the observed difference.
* **User Group Sizes:** Provides context on the number of users in each test group.
* **Visual Comparison:** A bar chart directly compares the conversion rates of the two groups.

**Based on the analysis, personalized messaging resulted in a 43% uplift in user engagement, a difference that was found to be highly statistically significant (p < 0.0001).**

## Data Source
The dataset used for this analysis is the "A/B Testing Data for a Conservation Campaign," sourced from Kaggle:
[A/B Testing Data for a Conservation Campaign on Kaggle](https://www.kaggle.com/datasets/tathagatachowdhury09/ab-testing-data-for-a-conservation-campaign)

The dataset includes user IDs, message type (Personalized/Generic), and engagement status (True/False). It contains 588,101 records.

## Tools & Techniques
* **Python (Pandas, SciPy):** Used for initial data loading, cleaning (removing unnecessary index columns), calculating conversion rates, performing the Chi-Squared test for statistical significance, and determining the uplift percentage.
* **Power BI Desktop:** Used for:
    * Data import and final data type verification.
    * Creating DAX measures to represent key metrics (e.g., `Conversion Rate Personalized`, `Conversion Rate Generic`, `Total Users Personalized`, `Total Users Generic`, `Uplift Percentage`, `P-value Display`).
    * Developing an interactive dashboard with KPI cards and comparative bar charts to visualize the A/B test results.

## Analysis Steps
1.  **Data Loading & Cleaning:** The dataset was loaded into a Pandas DataFrame, and an initial review of data types and missing values was conducted. The unnecessary index column was dropped.
2.  **Metric Calculation:** Conversion rates for both the "Personalized" and "Generic" groups were calculated.
3.  **Statistical Testing:** A Chi-Squared test for independence was performed to determine if the observed difference in engagement rates was statistically significant.
4.  **Uplift Calculation:** The percentage increase in engagement due to personalized messaging was quantified.
5.  **Dashboarding:** Key findings and metrics were visualized in Power BI to create an easy-to-understand summary of the A/B test results.

## Conclusion & Recommendation
The analysis conclusively shows that personalized messaging is significantly more effective at driving user engagement for this conservation campaign. It is recommended to implement personalized messaging strategies for future campaigns to maximize impact, given the observed 43% uplift.

## Skills Demonstrated
* A/B Test Analysis & Interpretation
* Statistical Significance Testing (Chi-Squared)
* Data Visualization (Power BI)
* DAX Measure Creation
* Data Cleaning & Preparation (Python/Pandas)
* Clear Communication of Analytical Results
