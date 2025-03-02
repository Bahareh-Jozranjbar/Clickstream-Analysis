# Clickstream Analysis  
**Author:** Bahareh Jozranjbar  

## Overview  
This project explores **clickstream analysis** to understand **user engagement patterns**, **predict behavior**, and **estimate dropout risk** using machine learning and survival analysis.  

Clickstream data provides insights into how users interact with digital platforms, revealing behavioral trends that traditional UX methods might miss. This analysis incorporates multiple techniques to **track user engagement, forecast future trends, predict behavior, and model dropout risk**.  

## Methods Used  
This project applies **four key approaches** to analyze clickstream data:  

1. **Tracking Engagement Trends**  
   - Identifies patterns in user interactions over time.  
   - Uses **scatter plots with trend lines** to show how average daily engagement relates to total clicks.  

2. **Forecasting Future Engagement (ARIMA Model)**  
   - Applies **time-series forecasting** to predict upcoming engagement trends.  
   - Uses an **ARIMA model** to generate future engagement estimates based on past clickstream data.  

3. **Predicting User Behavior (Machine Learning)**  
   - Trains a **Random Forest model** to predict user retention based on engagement features.  
   - Determines which variables (e.g., total clicks, engagement days) have the most impact.  
   - Outputs **feature importance rankings**.  

4. **Estimating Dropout Risk (Survival Analysis)**  
   - Uses **Kaplan-Meier survival curves** to model the likelihood of user disengagement over time.  
   - Implements a **Cox Proportional Hazards Model** to identify key factors influencing dropout risk.  

## Files Included  
- `clickstream_trends.png` – Engagement trends visualization  
- `feature_importance_rf.png` – Feature importance ranking from the Random Forest model  
- `km_survival_plot.png` – Kaplan-Meier survival curve for dropout analysis  
- `clickstream_forecast.png` – Time-series forecast of future engagement trends  

## Setup & Installation  
To run the analysis, install the necessary packages in R:  

```r
install.packages(c("data.table", "randomForest", "caret", "survival", 
                   "survminer", "ROSE", "keras", "ggthemes", "scales", "forecast"))
```


## Running the Analysis
The entire workflow is included in an R Markdown file (clickstream_analysis.Rmd). Follow these steps:

### Load and preprocess clickstream data.
- Train a Random Forest model to predict user retention.
- Perform survival analysis to estimate dropout risk.
- Generate time-series forecasts for future engagement trends.
- Export visualizations for interpretation.
  
To execute the script, open the .Rmd file in RStudio and run all chunks sequentially.

### Applications
This approach is valuable for product teams, UX researchers, and data scientists who want to move beyond surface-level analytics and uncover real behavioral patterns in user data.


