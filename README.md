# 📀 DVD Rental Duration Prediction

## Project Overview
This project aims to predict the number of days a customer will rent a DVD based on various features such as rental rate, replacement cost, and movie categories. The goal is to build a regression model that achieves a Mean Squared Error (MSE) of 3 or less on a test set, helping the rental company optimize its inventory planning.

This project was developed as part of a DataCamp challenge.

## Tools & Technologies
* **Python** * **Pandas & NumPy:** Data manipulation and feature engineering.
* **Scikit-Learn:** Machine learning modeling and evaluation.
    * *Lasso Regression:* Used for feature selection to eliminate non-informative variables.
    * *Ordinary Least Squares (OLS):* Baseline regression model.
    * *Random Forest Regressor:* Complex ensemble model for final predictions.
    * *RandomizedSearchCV:* Hyperparameter tuning.

## Methodology
1. **Data Preprocessing:** Calculated the rental duration in days and created dummy variables for specific movie features (e.g., deleted scenes, behind the scenes).
2. **Feature Selection:** Applied a Lasso Regression model to shrink irrelevant feature coefficients to exactly zero, keeping only the most impactful variables.
3. **Modeling:** Trained both a baseline Linear Regression model (using the Lasso-selected features) and a Random Forest Regressor.
4. **Evaluation:** Evaluated both models using Mean Squared Error (MSE) to ensure the target metric (< 3) was met.

## Results
* The **Random Forest Regressor** outperformed the baseline linear model.
* After hyperparameter tuning, the final model successfully achieved an MSE of less than 3 on the unseen test set, meeting the company's business requirement.

## How to Run
1. Clone this repository.
2. Ensure you have `pandas`, `numpy`, and `scikit-learn` installed in your environment.
3. Open and run the Jupyter Notebook to see the step-by-step analysis and model training.
