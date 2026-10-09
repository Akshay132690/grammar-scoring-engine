# Grammar Scoring Engine for Spoken Data

## About the Project

This project predicts the grammar score of a spoken audio recording on a scale of 0 to 5. I worked on extracting useful features from audio files and training machine learning models to predict grammar scores.

The project was developed as part of the SHL Hiring Assessment.

## What I Did

- Explored the training dataset and checked the distribution of grammar scores.
- Used Librosa to extract features from audio recordings.
- Extracted MFCCs, RMS energy, zero-crossing rate, spectral centroid, pitch, and other audio features.
- Trained and compared three machine learning regression models.
- Evaluated the models using RMSE and Pearson correlation.
- Selected the best-performing model and trained it on the complete training dataset.
- Generated predictions and saved them in a CSV file for submission.

## Models Used

- Random Forest Regressor
- Extra Trees Regressor
- HistGradientBoosting Regressor

## Tools and Libraries

- Python
- Pandas and NumPy
- Librosa
- Scikit-learn
- Matplotlib
- Kaggle Notebook

## Best Model

Among the models I tested, HistGradientBoosting with additional audio features performed best on my validation split.

- **Validation RMSE:** 0.7040
- **Pearson Correlation:** 0.8544

These results are from my validation data, not the final competition test set.

## What I Learned

Through this project, I gained practical experience in audio feature extraction, feature engineering, regression models, model evaluation, and generating predictions for unseen data.

## Note

The competition dataset and audio files are not included in this repository.
