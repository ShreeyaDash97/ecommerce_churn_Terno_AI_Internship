Predicting E-Commerce User Churn: A Practical Machine Learning Approach

In the fast-paced world of e-commerce, retaining users is a constant struggle. Every lost customer represents not only lost revenue but future growth potential walking out the door. That is why predicting churn—identifying users at risk of leaving—is critical for success. In this project, we leveraged a real user activity dataset to build and interpret a basic churn prediction pipeline.

The dataset tracks 50 users, logging how often they visit in the last month, how long they stay, how many purchases they made, and whether they raised a support ticket. 

Our goal: train a machine learning model that can alert us when a user is likely to churn.

First, we cleaned the data—coding churn and support ticket status into binary variables and checking for missing values (none!). Then, we explored the data. About 38% of users churned—a surprisingly high number! Digging deeper, churners made fewer purchases, visited less often, and spent slightly less time on site. Interestingly, users who raised support tickets were a little less likely to churn, suggesting that support might help retain users, though the effect was weak.

We trained a Logistic Regression classifier using visit frequency, site time, purchase count, and support status. The results were modest, with 40% accuracy—no better than guessing! The culprit? A small, slightly imbalanced dataset and very subtle feature effects. Still, our analysis highlighted key trends: users with low engagement and purchases are more likely to leave, while seeking support may help a few sticks around.

What does this mean for business? Even simple models can guide strategy. Proactively engaging users with few visits or purchases, and offering timely support, could reduce churn. With more historical data and richer features (e.g., marketing interactions, demographic details), predictive accuracy would soar.

In summary, AI for churn prediction is not a silver bullet, but a guidepost. It spotlights risky user groups, helps allocate retention efforts, and, when scaled up, powers actionable insights. For e-commerce teams, these models transform raw user data into business value—by turning churn into a preventable outcome.

