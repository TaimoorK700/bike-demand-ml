# BikeDemandML

## Overview
This project predicts bike-sharing demand using supervised machine learning on the UCI Bike Sharing Dataset.

## Dataset
The dataset contains hourly bike rental data with weather, time, season, and calendar variables.

## Project Goals
1. Predict exact hourly bike rental demand using linear regression.
2. Classify demand as low, medium, or high using logistic regression.

## Methods
- Exploratory data analysis
- Train/test split
- Linear regression
- One-hot encoding
- Feature engineering
- Error analysis
- Logistic regression classification
- Majority-class baseline comparison
- Balanced class weighting

## Key Results
### Regression
- Raw linear regression R²: 0.309
- One-hot encoded linear regression R²: 0.631
- Engineered linear regression R²: 0.721

### Classification
- Majority baseline accuracy: 40.6%
- Logistic regression accuracy: 82.5%
- Balanced logistic regression accuracy: 78.9%
- Balanced model improved high-demand recall from the original model.

## Key Findings
- One-hot encoding greatly improved linear regression performance.
- The model struggled most during commute/rush-hour periods.
- Adding morning/evening commute features reduced peak-hour error.
- Logistic regression performed much better than a majority-class baseline.
- Balanced logistic regression detected high-demand periods better, but reduced overall accuracy.

## Limitations
- Linear and logistic models may not capture all nonlinear demand patterns.
- The dataset is from one bike-sharing system and may not generalize to other cities.
- External factors such as events, station-level availability, and real-time disruptions are not included.

## Future Work
- Compare with decision trees, random forests, or gradient boosting.
- Add more advanced feature engineering.
- Build a simple dashboard or prediction interface.
