# Grammar Scoring Engine for Spoken Data

## Overview

This project explores the prediction of grammatical quality in spoken audio using machine learning regression techniques. The objective is to predict a continuous grammar score between 0 and 5 from audio recordings.

## Approach

The workflow consists of the following steps:

1. **Data Exploration:** Inspect the training data and analyze the distribution of grammar scores.
2. **Audio Feature Extraction:** Extract acoustic features from speech recordings.
3. **Feature Engineering:** Combine basic acoustic features with additional pitch, spectral, and speech-activity features.
4. **Model Training:** Train and compare multiple regression algorithms.
5. **Model Evaluation:** Evaluate predictions using Root Mean Squared Error (RMSE) and Pearson correlation on a validation set.
6. **Prediction:** Train the selected model on the complete training dataset and generate predictions for unseen samples.

## Audio Features

The extracted features include:

- Mel-Frequency Cepstral Coefficients (MFCCs)
- Root Mean Square (RMS) energy
- Zero-Crossing Rate
- Spectral Centroid
- Pitch statistics
- Spectral Bandwidth
- Spectral Rolloff
- Approximate Speech Activity Ratio

## Models Evaluated

- Random Forest Regressor
- Extra Trees Regressor
- HistGradientBoosting Regressor

The models are compared using validation performance to select the final approach.

## Technologies Used

- Python
- NumPy
- Pandas
- Librosa
- Matplotlib
- Scikit-learn
- Jupyter Notebook / Kaggle Notebooks

## Evaluation Metrics

**Root Mean Squared Error (RMSE):** Measures the difference between actual and predicted scores. Lower values indicate smaller prediction errors.

**Pearson Correlation:** Measures the strength of the linear relationship between actual and predicted scores. Values closer to 1 indicate a stronger positive relationship.

## Output

The final workflow generates a CSV file containing predicted grammar scores in the required submission format.

## Reproducibility and Data Usage

The code is intended to document the audio feature extraction and regression workflow. Competition datasets, audio recordings, and restricted prediction outputs are not included in this repository.

Use only data that you are authorized to access and distribute, and follow the applicable competition rules.

## Disclaimer

This project was developed as part of a machine learning assessment workflow. Results depend on the dataset, feature extraction process, validation split, and model configuration.
