#Student Performance Predictor

#Project Overview

This project focuses on building a machine learning model to predict a student's final grade based on key behavioral and historical metrics. This is a Regression task, where the goal is to predict a continuous numerical value (the grade, $0-100$).

The project demonstrates data generation, exploration, and the application of an advanced ensemble model to achieve high predictive accuracy.

#Key Results and Model Performance

The final model used for prediction was the Random Forest Regressor. This ensemble method was chosen because of its superior ability to handle non-linear data patterns, significantly outperforming simpler models like Linear Regression.


Technology Stack

Language: Python

Data Handling: Pandas, NumPy

Machine Learning: Scikit-learn (RandomForestRegressor, train_test_split, r2_score)

Visualization: Matplotlib, Seaborn

Project Stages

Phase 1: Data Generation & Exploration

Data Source: Synthetic data (100 students) generated using NumPy, simulating real-world student behavior.

Features: study_hours, attendance, and previous_grade.

Target: final_grade, calculated using weighted scoring based on feature importance and clipped between $0$ and $100$.

Phase 2: Correlation Analysis

A correlation heatmap was used to confirm the relationship between the features and the target, validating that study_hours was the dominant predictive factor.

Phase 3: Model Building & Evaluation

The data was split $80/20$ into training and testing sets.

The Random Forest Regressor was trained on the data.


Visualization of Predictions

The scatter plot below shows the model's performance on the test set. Points clustered tightly around the red "Perfect Fit" line indicate high accuracy.

Note: The narrow clustering of points around the red line visually confirms the high R² accuracy.
