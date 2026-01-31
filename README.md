Spotify Song Popularity Prediction

Regression analysis of artist, track, and album features to model song popularity.

Overview

This project models Spotify track popularity using artist-, track-, and album-level metadata collected via Spotify’s API. The goal is to understand which characteristics most strongly influence a song’s popularity score and how these factors interact across artists with different levels of existing popularity.

Using multiple linear regression, the analysis compares artist-only, track-only, combined, and interaction-based models to evaluate predictive accuracy and uncertainty. Results highlight the dominant role of artist popularity while illustrating the limitations of metadata-only approaches for predicting cultural success.

Objectives

Analyze how artist characteristics relate to Spotify track popularity

Assess the predictive value of track and album features

Compare multiple regression model specifications

Evaluate model performance using RMSE, R², and prediction intervals

Examine interaction effects between artist popularity and track attributes

Methods & Tools

Tools & Libraries:
R • tidyverse • glmnet • tidyr

Techniques:

Data cleaning and transformation (log scaling, factor encoding)

One-hot encoding of artist genres

Train/test data splitting

Multiple linear regression modeling

LASSO regularization for feature selection

Bootstrap-based prediction intervals

Residual diagnostics and model comparison

Key Findings

Artist popularity and follower count were the strongest predictors of track popularity.

Track- and album-level features alone explained relatively little variation in popularity.

Models including interaction effects between artist popularity and track features performed best.

Even the best-performing model showed substantial uncertainty, reflecting the inherent difficulty of predicting song popularity using metadata alone.

Limitations & Insights

Predictive performance was moderate, with a large portion of variance in popularity remaining unexplained.

Wide prediction intervals highlight uncertainty and limited precision.

External factors such as playlist placement, marketing, and viral trends are not captured by the data but likely play a major role.

Skills Demonstrated

Regression modeling and model comparison

Feature engineering and data transformation

Regularization and feature selection (LASSO)

Model diagnostics and uncertainty quantification

Statistical reasoning and technical reporting
