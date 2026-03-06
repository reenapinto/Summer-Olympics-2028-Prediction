# Summer Olympics 2028 Medal Prediction

## Project Overview
This project predicts country-level and sport-level medal counts for the 2028 Summer Olympics using historical Olympic medal data, athlete participation, population, and GDP per capita.

## Objectives
- Clean and prepare Summer Olympics historical data
- Engineer predictive features at the country-sport-year level
- Train machine learning models to predict Gold, Silver, and Bronze medals
- Generate medal forecasts for the 2028 Summer Olympics
- Visualize predicted rankings and feature importance

## Dataset Sources
- Historical Olympic medal dataset
- Athlete events dataset
- Population dataset
- GDP per capita dataset

## Project Structure
- `notebooks/01_data_cleaning.ipynb` → data cleaning and feature engineering
- `notebooks/02_modeling_2028_prediction.ipynb` → model training, validation, prediction, visualization
- `outputs/` → final cleaned tables and prediction files
- `images/` → saved charts for GitHub display

## Features Used
- Previous sport medals
- Athlete count
- Host advantage
- Log population
- Log GDP per capita

## Modeling Approach
The project uses XGBoost with a Poisson objective to predict medal counts for:
- Gold
- Silver
- Bronze

## Key Outputs
- Country-level medal predictions for 2028
- Sport-level medal predictions for 2028
- Validation plots comparing actual vs predicted medals
- Feature importance analysis

## Sample Visualizations

![Top 15 Predicted Medal Winners](images/top15_pred_total_2028.png)

![Feature Importance](images/feature_importance_gold.png)

## Key Insights
- Previous sport-level medal history is the strongest predictor of future medals.
- GDP per capita and population contribute positively but with diminishing returns.
- Host advantage boosts medal predictions for the United States in 2028.
- Medal efficiency analysis highlights smaller countries that overperform relative to population.

## Limitations
- Historical macroeconomic data required forward-filling and imputation for some countries.
- Athlete count is used as a proxy for participation strength.
- Predictions reflect historical trends and do not account for injuries, qualification changes, or future policy shifts.

## How to Run
1. Run `01_data_cleaning.ipynb`
2. Run `02_modeling_2028_prediction.ipynb`
3. Check outputs in the `outputs/` folder

## Author
Reena Pinto
