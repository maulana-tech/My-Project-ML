# Music Popularity Prediction with Python

This project focuses on predicting the popularity of songs using various music features and metadata. It employs regression techniques to forecast a song's performance in terms of streams, downloads, and chart positions. The goal is to provide music producers, artists, and marketers with accurate predictions to make informed decisions.

## Overview

The project uses a dataset of Spotify tracks to build a regression model that predicts song popularity. The analysis involves:

1.  **Exploratory Data Analysis (EDA):** Visualizing the relationships between music features (like energy, danceability, and acousticness) and popularity.
2.  **Feature Selection:** Identifying the most influential features for predicting popularity based on correlation analysis.
3.  **Model Training:** Training a Random Forest Regressor model on the selected features.
4.  **Hyperparameter Tuning:** Using GridSearchCV to find the optimal parameters for the model.
5.  **Evaluation:** Assessing the model's performance by comparing its predictions to the actual popularity scores.

## Dataset

The dataset used in this project is `Spotify_data.csv`, which contains various features for each track, including:

*   **Track Name:** The name of the song.
*   **Artists:** The artists of the song.
*   **Album Name:** The album the song belongs to.
*   **Popularity:** The popularity score of the song (the target variable).
*   **Acoustic Features:** Energy, Valence, Danceability, Loudness, Acousticness, Tempo, Speechiness, and Liveness.

## Analysis and Model

The analysis begins with an exploratory data analysis (EDA) to understand the relationships between different musical features and popularity. The correlation matrix and visualizations show that features like `Energy`, `Danceability`, `Loudness`, and `Acousticness` have a significant correlation with popularity.

Based on this analysis, the following features were selected for model training:
- Energy
- Valence
- Danceability
- Loudness
- Acousticness
- Tempo
- Speechiness
- Liveness

A Random Forest Regressor was chosen as the prediction model after comparing its performance with other algorithms. The model was trained on the selected features, and `GridSearchCV` was used for hyperparameter tuning to find the best model parameters.

## Results

The trained model shows a good correlation between the actual and predicted popularity scores, as seen in the scatter plot of the results. This indicates that the model can effectively predict music popularity based on the given features.

![Actual vs Predicted Popularity](httpsT4m6PAarQQMz)

## How to Run

To run this project, you can use the Jupyter Notebook `ML_01_Music_Popularity_Prediction_with_Python.ipynb`. Make sure you have the following libraries installed:

*   pandas
*   matplotlib
*   seaborn
*   scikit-learn

You can open the notebook in a Jupyter environment or Google Colab and run the cells sequentially to see the analysis and model training process.
