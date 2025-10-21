📈 Insurance Claim Fraud Prediction Model
Note: I am actively building out this solution. All constructive critique, advice on methodology, or suggestions for improving feature engineering are highly welcomed. Thank you for taking the time to view my work.

Project Status: 🚧 Active Development (Work-in-Progress)
1. Project Objective
This project aims to develop a robust XGBoost Classification Model to identify fraudulent insurance claims with high accuracy. Given the inherent class imbalance of fraud datasets, the primary performance focus is maximizing Sensitivity (Recall) to minimize the number of missed fraudulent claims, while maintaining a strong Area Under the Curve (AUC) score.

2. Technical Stack
Category: Tools/Libraries Used
Language: Python (3.x)
Data Manipulation: pandas, numpy
Modeling & ML: XGBoost, scikit-learn
Visualization: seaborn, matplotlib, plotly (for geospatial analysis)
Statistical Analysis :scipy.stats, statsmodels

✅ Accomplished (Phase 1)
Data Preparation: Loaded, cleaned, and performed initial preprocessing on the insurance claims dataset.

Exploratory Data Analysis (EDA): Conducted analysis to understand feature distributions, correlations, unnecessqry variables, and initial insights, documented in insurence_project_eda.ipynb.

Baseline Modeling: Trained and evaluated an XGBoost model using grid search.

Performance Evaluation: Established baseline model performance using robust metrics critical for imbalanced data, including ROC AUC (0.85) and Confusion Matrix analysis.

Future Roadmap 
Imbalance Mitigation: Implement bootstrapping or advanced resampling techniques (e.g., SMOTE) to effectively manage the 3:1 class imbalance during training, aiming to stabilize the model and improve minority class performance. (Percision and recall are not too good)

Model Explainability: Introduce SHAP (SHapley Additive exPlanations) to provide local and global interpretation of model predictions, moving beyond simple feature importance.

Advanced Feature Engineering: Utilize the insights gained from SHAP analysis—specifically, identifying key feature interactions—to guide the creation of new, high-impact features to significantly boost the final model's predictive power.


