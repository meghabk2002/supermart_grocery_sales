📊 Project 
Overview
This project focuses on building a predictive model using Random Forest Regression to estimate the profit generated from grocery sales in a retail business. 
The dataset contains transactional data including product categories, geographic region, sales details, and order dates.
A machine learning pipeline is constructed using scikit-learn, with preprocessing steps for handling categorical variables and engineered features derived from the order date and sales values. 
The end goal is to help stakeholders understand and predict profit behavior across various business dimensions.

🎯 Objective
To predict Profit based on multiple sales and categorical features using a Random Forest Regressor.
To extract actionable insights into which factors (e.g., state, discount, category) influence profit the most. 
To evaluate the performance of the model using key regression metrics (MAE, RMSE, R²).
To export and visualize predictions for further business analysis.

🔍 Key Insights
Feature Engineering:
Extracted temporal features like Month and DayOfWeek from Order Date.
Created a new feature Net Sales to better reflect post-discount sales revenue.
Calculated Profit Margin to capture sales efficiency.

Data Preprocessing:
Missing dates were handled gracefully.
Used OneHotEncoding to convert categorical columns like Category, Sub Category, Region, and State into numerical format for modeling.

Model Performance (on Test Set):

Mean Absolute Error (MAE): Measures average prediction error in profit.
Root Mean Squared Error (RMSE): Punishes large errors more, useful for business risk evaluation.
R² Score: Shows how well the model explains variance in profit (typically values above 0.7–0.8 indicate strong performance).

Model Deployment Preparation:
Final predictions are combined with test data and exported as a .csv file (rf_predictions.csv), enabling downstream use for reporting or dashboards.

✅ Conclusion
A well-performing Random Forest model was successfully built to predict retail profit with reasonable accuracy.
The pipeline approach ensures scalability and reproducibility.
The most influential features in predicting profit are likely to be state, discount, and net sales, which can be further analyzed using feature importance techniques.
The exported predictions can help business stakeholders identify high-risk regions, underperforming product categories, or ineffective discount strategies.
