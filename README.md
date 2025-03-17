# Traffic Collision Fatality Analysis

## Kaggle Competition - 4th Place Rank

As part of a Kaggle competition, my team and I developed a machine learning model to predict the severity of traffic collisions. Out of many competing teams, we secured **4th place** with our high-performing model.

## Project Overview
- **Dataset:** Police-reported traffic collisions (2006-2022), with 15,000+ records and 54 features.
- **Objective:** Predict whether a collision results in a fatal or non-fatal injury.

## Approach & Key Steps

### 1. Data Preprocessing
- Concatenated street-related features.
- Dropped unnecessary columns (e.g., OBJECTID, DATE, TIME).
- Imputed missing values using "Unknown," median, and mode.
- Applied **One-Hot Encoding** for categorical variables.

### 2. Model Selection & Training
- Implemented multiple models, including:
  - **Random Forest Classifier** (Best performer)
  - K-Nearest Neighbors (KNN)
  - Logistic Regression
  - Naïve Bayes
- Used **Stratified Train-Test Split** (75:25 ratio).
- Fine-tuned hyperparameters with **Grid Search CV**.

### 3. Performance Evaluation
- **ROC Curve & AUC:** Random Forest had the highest AUC.
- **Confusion Matrix Analysis:** Adjusted threshold from 0.5 to 0.05, improving recall from 0.55 to 0.96.
- **Final Kaggle Score:** Achieved 90.39% accuracy on the test dataset.

## Key Takeaways
- Feature engineering significantly improved model performance.
- Random Forest outperformed other models but required threshold tuning.
- Hyperparameter tuning (Grid Search CV) optimized performance but slightly reduced accuracy due to validation set overfitting.

## Outcome
Our optimized machine learning model achieved **4th place** in the Kaggle competition, demonstrating strong analytical and predictive modeling skills.
