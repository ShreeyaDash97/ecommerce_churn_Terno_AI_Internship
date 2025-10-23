1. Which user activity features are most correlated with churn?
VisitsLast30Days, TimeOnSite, PurchaseCount: All have weak negative correlations with churn. This means users who visit less, buy less, and spend less time are slightly more likely to churn.

Model coefficients:

VisitsLast30Days: -0.033

TimeOnSite: -0.088

PurchaseCount: -0.179

PurchaseCount is the most correlated (largest negative value), followed by TimeOnSite and then VisitsLast30Days.

2. How does raising a support ticket affect churn probability?
HasSupportTicket coefficient: +0.010 (very weak, almost neutral)

Users who raise support tickets are only very slightly less likely to churn according to model analysis; the effect is extremely weak in your sample.

3. What are the typical profiles of users who churn?
Make fewer purchases (mean ~4.53 vs 5.03 for non-churners)

Visit less (22.58 vs 27.35 in the last 30 days)

Spend less time per session (11.21 vs 12.00 minutes)

Slightly less likely to raise support tickets

4. Which feature(s) are most predictive of churn?
PurchaseCount is the most predictive, with the largest coefficient magnitude (-0.179). Less purchasing activity means higher probability of user churn.

5. What is the overall churn rate?
Churned: 19 of 50 users (from value counts in your notebook)

Churn rate: 38%

Summary:

Users who buy less, visit less, and spend less time are most at risk.

Support tickets have little effect on churn probability in this dataset.

Overall, about 38% of users churned in your sample.