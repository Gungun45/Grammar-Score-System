🧠 Project Title: Grammar Scoring Engine for Spoken Audio
📌 Project Description:
This project focuses on building a Grammar Scoring Engine capable of evaluating spoken English grammar from 45–60 second audio clips. Given a dataset of .wav files along with MOS Likert-based grammar scores ranging from 0 to 5, the objective is to create a machine learning model that predicts a continuous grammar score for any new audio input.

🎯 Objective:
To develop a machine learning pipeline that:

Processes and extracts relevant features from audio files.

Trains a regression model to predict grammar scores.

Evaluates performance using RMSE (Root Mean Squared Error).

Submits predictions for the test dataset in the required format.

🗂️ Dataset Overview:
train.csv: Contains filenames and their grammar scores.

test.csv: Contains filenames of audio files (labels hidden).

sample_submission.csv: Sample format for submission.

Audio Files: .wav format with speech recordings.

📈 Modeling Approach:
Audio Preprocessing: Feature extraction using MFCCs (Mel Frequency Cepstral Coefficients).

Regression Model: Trained a RandomForestRegressor to predict continuous grammar scores.

Validation: RMSE used as the primary metric. Predictions are clipped between 0 and 5.

📊 Evaluation Metric:
Root Mean Squared Error (RMSE) on validation set.

Leaderboard Metric: Pearson Correlation (for final submission).
