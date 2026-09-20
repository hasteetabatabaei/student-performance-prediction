1. Student Performance Prediction using XGBoost

This project predicts the final math grade ('G3') of secondary school students
based on demographic, social, and academic features.

2. Key Machine Learning Highlight: Preventing Data Leakage
During initial modeling, including first ('G1') and second period ('G2') grades
resulted in an optimistic MAE of **1.1812**.
 However, realizing that G1 and G2 act as target-proxies and cause **Data Leakage**,
they were removed to build a **realistic predictive model** based solely
 on student background and habits.

3. Tech Stack & Methods
- **Python** (Pandas, NumPy, Matplotlib)
- **Scikit-Learn** (OrdinalEncoder, Train/Test Split)
- **XGBoost** (Gradient Boosting with Early Stopping)

4. Results
- **Initial MAE (with G1/G2 - Leaky Model):** ~1.18
- **Realistic MAE (without G1/G2):** ~3.58 (out of 20 points)

5. Top Feature Importances
Removing previous grades revealed that features like **past class failures**,
 **school absences**, and **study time** are key indicators of final student success.
