# Columbia Engineering competiton: Predicting Click-through Rates
## Ensembled 12 CatBoost, XGBoost, LightGBM models using Stacking, with Elastic-Net Logistic Regression as meta-model

I competed in a team of 3 in a Columbia Engineering competition open to Masters students, and placed 4<sup>th</sup> out of 200 participants.
<li>Applied numerous categorical feature encoding methods on dataset with purely categorical features.
<li>Extensive feature engineering to capture temporal nature of consumer clicks.


#About
This competition was adapted from Avazu's highly popular Kaggle competition in 2015, linked 
<a href="https://www.kaggle.com/c/avazu-ctr-prediction" target="_blank">here</a>.

Avazu is a programmatic advertising platform that uses machine learning to decide which mobile advertisements get pushed to which consumers. Its aim is to maximize advertising effectiveness by ensuring the correct target group receieves the advertisements they are most interested in.

This competition is to predict consumer click-through rates on mobile advertisements, ie. whether a consumer clicks on an advertisement.

In online advertising, click-through rate is a very important metric for evaluating ad performance and is used in sponsored search and real-time bidding.


# Data
This competition uses 4 million rows with ~30 features that contain information about the consumer's mobile device, the mobile advertisement, the website on which the advertisement was encountered, etc. Each row depicts a specific user on a specific mobile device, encountering a specific mobile advertisement, and the target of whether the user clicked on it.


# Project Methodology
1. Obtain training and test sets via time split: Due to time nature of data
2. Feature engineering to identify unique consumers from device data
3. Feature engineering to extract time nature of data
4. Feature cleaning of rare values
5. Encode categorical features: Using Hash Encoding, Ordered Target Encoding, Ordinal Encoding
6. Train & tune model hyperparameters using Bayesian Optimization: CatBoost, XGBoost, LightGBM
7. Ensemble models: Using Stacking, with Elastic Net Logistic Regression as meta-model
8. Re-run on full data


# Still curious?
Check out this project on my website <a href="https://sheilateozy.github.io/#portfolio" target="_blank">here</a> :)


