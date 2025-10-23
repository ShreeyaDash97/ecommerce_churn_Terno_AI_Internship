# ecommerce_churn_Terno_AI_Internship
Build a machine learning model to predict whether an e-commerce user will churn (leave the platform), based on their recent site activity and support ticket status.
1. Problem Statement
Predict user churn in an e-commerce setting, using behavioral and support data.
Churn (losing customers) is a major business challenge. We use recent visit frequency, time spent, purchasing behavior, and support ticket status to train a model identifying likely churners.
2. Data Cleaning & Preprocessing
No missing values.
All categorical variables (Churned, HasSupportTicket) are now encoded as 0/1.
3. Exploratory Data Analysis (EDA)
Churn rate: 38% (19 out of 50 users churned)
Support ticket effect:
42% churn rate for users without support tickets
35% churn rate for users with support tickets
Feature means:
Churned users make fewer purchases (4.5 vs 5.0), visit less often (22.6 vs 27.3), and spend a bit less time (11.2 vs 12.0 minutes).
Correlation analysis:
All features have weak negative correlation with churn, meaning lower values are associated with higher churn.
4. Machine Learning Model
Type: Logistic Regression (classification)
Accuracy: 40% on test set (sample is small)
Confusion Matrix:
Model only predicts "No churn" in test set
Classification Report:
Precision for “No churn”: 0.4, Recall: 1.0
Precision for “Churn”: 0.0, Recall: 0.0
Model coefficients:
VisitsLast30Days: -0.03
TimeOnSite: -0.09
PurchaseCount: -0.18
HasSupportTicket: +0.01
Interpretation:
All activity features slightly decrease churn probability, but effect is weak in this sample.
5. Questions Answered
Which features are most important for predicting churn?
PurchaseCount and TimeOnSite are most predictive (but weak).

Does raising a support ticket reduce churn?
Slightly, but effect is weak.

How accurate can the model get?
40% with this small, imbalanced dataset.

Profile of churners:
Fewer visits, fewer purchases, less time on site, fewer support tickets.
