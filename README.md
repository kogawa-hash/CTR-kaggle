Description:

In the rapidly evolving landscape of digital marketing, businesses strive to drive traffic to their websites to maximize consumer engagement with website content and for online retailers also promote sales. Display advertising is one method used to drive traffic. Success of a display ad is judged by the percentage of visitors who click on the ad, commonly known as Click-Through Rate (CTR). The goal of this competition is to predict CTR based on a set of variables describing the quality, relevance, type, target audience, and content of the display advertisement.

Goal:

Construct a model to predict CTR based on features of the display ad and use it to generate predictions for a set of unlabeled data.
Submissions will be evaluated based on RMSE. 

Process:

- conduct data cleaning. For numerical variables, impute columns with NA values with their median values. For categorical variables, impute NA values with their modes. Convert all categorical columns to numeric types using label encoding to keep the consistency of data types across data set.
- screen predictors by examining their bivariate correlations to CTR. Using a correlation matrix, identify four variables—targeting_score, visual_appeal, cta_strength, and headline_length.
- run xgboost with hyperparameter tuning varying key parameters such as learning rate, max depth, and column sampling ratios. Experiment with different cross-validation (CV) folds.
- implement early stopping during training to prevent overfitting.
- measure rmse score

Results:

RMSE = 0.062

ranked 14 out of 360 participants


