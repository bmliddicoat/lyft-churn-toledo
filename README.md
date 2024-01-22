# lyft-churn-toledo

# Lyft Pricing Strategy Analysis

## Overview

This project involves a detailed analysis of Lyft's pricing strategy for a ride-scheduling feature in Toledo, Ohio. The focus is on determining the optimal driver payment (by adjusting Lyft's take per trip) to maximize net revenue over the next 12 months, considering various factors such as match rates, driver and rider churn rates, and Customer Acquisition Costs (CAC).

## Data and Assumptions

### Key Parameters

* Prevailing Rates: Riders pay $25 per ride; drivers earn $19 per ride.
* Driver and Rider Churn Rates: Drivers have a 5% monthly churn rate; riders churn at 10% normally and 33% if they experience a failed match.
* CAC: $400 - $600 for drivers and $10 - $20 for riders.
* Match Rates: Vary based on Lyft's take; a reduction in Lyft's take from $6 to $3 increased match rates from 60% to 93%.
* Assumptions: Linear relationship between Lyft's take and match rates, capped at 100%.
  
## Analysis Approach

* Modeling Match Rates: Based on experiment data, a linear model was created to estimate match rates for varying Lyft takes.
* Net Revenue Calculation: Calculated by considering the total revenue, churn rates, and CAC for different scenarios of Lyft's take.
* Visualization: Plotted Match Rate vs. Lyft Take and Net Revenue vs. Lyft Take for a clearer understanding of trends.
  
## Key Findings

* Match Rates: There's a significant increase in match rates as Lyft's take decreases.
* Net Revenue: All scenarios showed negative net revenue, suggesting the need for broader strategic changes beyond pricing adjustments.
* Optimal Pricing Strategy: The analysis suggests that pricing alone may not be sufficient to achieve positive net revenue under the current cost structure.
  
# Recommendations

* Cost Structure Review: Reevaluate the cost structure, including CAC and operational expenses.
* Market Dynamics: Consider external factors such as competition and seasonal variations.
* Data-Driven Decisions: Use more detailed data, especially on ride frequency and driver behavior, for further analysis.

## Technologies Used

* Python
* Libraries: NumPy, Pandas, Matplotlib
