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

3. Methodology & Current Progress
The project follows a standard machine learning workflow. The Exploratory Data Analysis (EDA) phase is complete, and the focus is shifting to advanced feature engineering and model preparation.

Completed: Initial EDA & Data Cleaning
Custom Missing Value Imputation: Identified and systematically handled non-standard missing data placeholders (?) by converting them to np.nan for accurate analysis.

Missingness Significance: Performed Chi-Squared Tests to confirm that the missingness of key categorical features (e.g., police_report_available) is statistically dependent on the target variable (fraud_reported). This justifies treating missingness as a valuable feature category for the tree-based model.

Next Steps: Detailed To-Do List
Phase	Task	Details
Feature Engineering	
  1. Temporal Feature Creation	Deriving crucial variables: 'Car Age' and 'Customer Tenure' (time between policy bind and incident date) to capture temporal risk factors.
  2. Geospatial Analysis (EDA)	Implementing a Choropleth Map visualization to identify potential geographic clusters of high fraud rates by state or region.
    Feature Encoding
  3. High-Cardinality Strategy	Applying Target Encoding to high-cardinality nominal features (e.g., auto_model, insured_hobbies) to manage dimensionality while preserving predictive power.
  4. Addressing Imbalance	Mitigating the class imbalance issue using the scale_pos_weight hyperparameter within the XGBoost model training phase.
  Model & Evaluation
  5. Model Training & Tuning	Training the XGBoost classifier and optimizing hyperparameters via cross-validation.
  6. Comprehensive Evaluation	Full assessment using AUC, Sensitivity (Recall), and Specificity as primary metrics.
  Post-Modeling
  7. Feature Importance Analysis	Generating a final report detailing the most significant predictors identified by the model to provide actionable business intelligence.


