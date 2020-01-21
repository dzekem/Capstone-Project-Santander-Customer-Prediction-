
# Santander Customer Predictions

## Problem Statement

Customer preservation is essential in a variety of businesses as acquiring new customers is often
costlier than keeping the current ones. Many companies are therefore always trying to answer the
question “How can we predict the value of a customer over the course of his or her interactions
with the business”. Santander therefore wants to know future customer transaction predictions.

## Methodology

This project will undergo a series of processes outlined as:
• Exploratory Data Analysis where the different relationships between the 200 features and
the target
• Inferential Statistics applied on the different features and the target.
• After these analyses, stories will then be brought out from these results depending on the
visualizations gotten.
• Since this project is a classification problem with two classes (0 and 1), different machine
learning classification models will be tested on the dataset to see which best predicts with highest
model accuracy score.

## Exploratory data analysis

Doing exploratory data analysis on both the data frame, so much information was extracted from
it which brings out so much insights from the data.
From the description of this data frames, Standard Deviation being a measure that is used to quantify the amount of variation.   
This implies a low Standard Deviation value indicates that data points turn to be close to mean while a high Standard
Deviation value shows data points are spread out over a wide range of values.

Visualizing the relationship between each feature and the target using density plots of all the 200 features shows sum of all 
probabilities with the peak of the density plot showing the highest probability of the data points.
Since the aim of this project is to predict customers that will make a transaction in the future, like 5% of the features 
have the peak value at a probabilistic level of 0.6 which is the highest.

## Inferential Statistics

From this analysis, the Pearson correlation makes the var_91 feature statistically important as this feature could be used to 
increase future customer transactions which is the aim of this project. If for instance this feature was a coupon or some 
bonuses, increasing these offers if increased could therefore increased the probability of having a customer make a future 
transaction.

## Applying Machine Learning Algorithms

Two models will be used to make predictions so as to choose the one with best accuracy score as the most suitable one. The 
models considered are;
1. Logistic Regression with and without regularization
2. Gaussian Naïve Bayes model

- Applying Logistic Regression on the data set produced good accuracy scores for both training and test data. But when 
displaying a classification report, the precision values for both classes has a large difference as the data is imbalance.
- For Gaussian Naïve Bayes, the model is overfitting because the training and test accuracies have a large difference which 
implies the model is too complex for the dataset.
- Therefore, the best algorithm for this case is Logistic Regression which is implemented after the data has been made 
balanced. This therefore solves the problem of Imbalance data which was faced because of the great difference in the two 
classes.

## Client Recommendations

• Considering the three features with highest probability values of having a customer make a future transaction in the 
future. These features are var_91, var_108 and var_148 produce the highest probability values of having a 1 as target. These 
features though anonymous could therefore be used to further increase this probability by ensuring values equivalent to their 
mean or higher.
• Also, the features with lowest probability values like var_5, var_84 and var_86 are the one of the features causing the 
customers not to make a future transaction in the future. These features which are unidentified could further be used by 
ensuring they instead contribute to a higher probability of having a 1 as the target.
• From this analysis, the average number of customers transaction per day, week or month could be calculated and from this 
the company will know if they are meeting up with the target ahead of them or not. And if the target is not being met, they 
can therefore bring forth improvements to this by offering bonuses and more promotions which will increase customer awareness 
about their products and services.

