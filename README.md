# tiktok-video-engagement-prediction
# TikTok Video Engagement Prediction (Day 30 View Count)

## Project Overview
This repository contains the Machine Learning pipeline built for the In-Class Kaggle Competition to predict cumulative 30-day TikTok video views using the first 5 days of engagement data.

## Key Technical Steps
- **Target Transformation**: Used `log1p` transformation to handle the skewed Power Law distribution and stabilize RMSE evaluation.
- **Feature Engineering**: Extracted cumulative interaction stats, growth velocity, and ratio metrics (likes/views, shares/views, comments/views) from Days 0 to 5.
- **Modeling**: Trained a LightGBM Regressor using 5-Fold Cross-Validation.
- **Evaluation Metric**: Root Mean Squared Error (RMSE).

## Repository Files
- `TikTok_Prediction.ipynb`: Complete reproducible pipeline code.
- `submission.csv`: Final target predictions for Kaggle leaderboard.
