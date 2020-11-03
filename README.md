# promotions
My team analyzed what affects an employee to get a promotion and created models to predict promotions.

Most people work hard to get promoted, but not everyone will get it. With promotions come a salary increase, maybe some extra perks, and definitely a sense of achievement. However, if you don’t get the promotion, then disappointment may start to creep in. Is there a secret to being promoted? Is there a way to know if you get the promotion? That is what we are trying to determine in this project.

Our data was taken from a multinational corporation and everyone in our dataset was put up for promotion. Then these people were put through a training and given a score, which was taken into account on if they would get the promotion. About 8.5% of these people were actually promoted. Overall, we had 54,808 individuals with 14 different columns describing them. These columns include KPIs met>80%, awards won?, department, previous year rating, and more. Figure 1 illustrates more about our data and to learn more about the columns click this link: https://www.kaggle.com/rsnayak/wns-analytics-wizard-2018-ml-hackathon#0.2.-Objective:

We decided to create models using only male and only female workers to see if there was going to be a difference in the important deciding factors. We also decided to fit three models to our data and see which one had the best predictions. The first model we ran was a logistic regression model, which can be thought of as the analog to linear regression for classification problems. The second model we built was a K-Neareast Neighbors Classifier model, which makes predictions based on similarities in values to other people. Our third and last model was XGBoost. The XGBoost model makes predictions by subsequently building a number of decision trees. The trees are built in an additive manner, meaning each tree is built based on the previous tree’s mistakes.

Based on these three models and their f1-scores, we decided that the XGBoost model was the best at making predictions overall.

The two areas where this model misses the most is when employees meet 80% of their KPIs at 20.5% and when employees win awards at 24.6%. In future research, we could look at these columns more in depth and possibly create more models separating the values in these columns to see if our model improves.

Our data can be found here: https://www.kaggle.com/arpina/promotion?select=promotion.csv

The article for this project can be found here: https://www.linkedin.com/pulse/promotions-climb-corporate-ladder-stephanie-lao/?trackingId=OvAC1POkTZiLQOz0g9lnEQ%3D%3D
