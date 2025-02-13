# Databusters-Economic-Contraction-Prediction

# Project Overview
This project focuses on forecasting U.S. economic contractions using macroeconomic indicators and machine learning techniques. The goal is to predict whether the economy will experience a downturn in the next 3, 6, or 12 months, helping policymakers and analysts take proactive measures.

# Dataset
Monthly & Quarterly Macroeconomic Data: Includes GDP, unemployment rate, interest rates, consumer spending, and other economic indicators.

Source: Federal Reserve Economic Data (FRED).

Time Period: Historical economic data used to train and validate models.

# Methodology
1. Data Cleaning & Preprocessing
Handled missing values based on severity (forward-fill, interpolation, regression imputation).
Dropped highly correlated features using Variance Inflation Factor (VIF) to address multicollinearity.
Engineered new features such as inverted yield curves and housing investment ratios.
Performed Principal Component Analysis (PCA) to reduce dimensionality.
2. Extrapolation for 2025 Predictions
Used linear regression to predict missing economic indicators for 2025, allowing the models to make future predictions.
3. Model Selection & Training
Random Forest Classifier: Used for short-term forecasting due to its robustness and ability to handle high-dimensional data.
Long Short-Term Memory (LSTM): Applied to capture long-term dependencies in time series data.
4. Evaluation Metrics
F1-score: To balance precision and recall in detecting economic contractions.
Precision & Recall: To evaluate false positives/negatives in contraction predictions.
Confusion Matrix: To visualize model performance.

# Results & Findings
Random Forest Model achieved high accuracy on training data but struggled with imbalanced classes in testing, leading to low recall for contractions.
LSTM Model performed better at capturing trends, with an F1-score of 0.85 for 3-month predictions.
Feature importance analysis highlighted key predictors, including unemployment rate, consumer sentiment, and the yield curve inversion.

# Technologies Used
Python (Pandas, NumPy, SciKit-Learn, TensorFlow, Matplotlib, Seaborn)
Machine Learning Models: Random Forest, LSTM
Time-Series Forecasting: Linear Regression for extrapolation

# Future Work
Improve class balancing techniques (SMOTE, weighted loss functions).
Experiment with XGBoost and Transformer models for better long-term forecasting.
Incorporate real-time economic data for continuous learning.

# Contributors
Team DATABUSTERS 13 – NUS DSESC Challenge

# Acknowledgments
Special thanks to NUS Data Science & Economics Club and competition organizers for providing the dataset and research framework.
