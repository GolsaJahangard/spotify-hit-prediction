# Spotify Hit Prediction using Artificial Neural Networks

Deep learning project for predicting Spotify song popularity using feature engineering and Artificial Neural Networks.

This project started as a deep learning assignment, but I treated it as an opportunity to build a complete machine learning pipeline instead of only training a neural network.

The goal is to predict a song's hit potential using only its audio features. The dataset contains more than 1.1 million Spotify tracks, and the project covers everything from data preprocessing and feature engineering to model training, evaluation, and a simple prediction simulator.

## What I did

- Explored the dataset and analyzed feature importance
- Removed highly correlated features
- Removed outliers using the Z-Score method
- Applied cyclical encoding for musical keys
- Frequency encoded the `genre` feature
- Created a custom three-class hit labeling strategy
- Built and trained a deep Artificial Neural Network using TensorFlow/Keras
- Compared training on 5% of the data versus the full dataset
- Evaluated the model using learning curves and a confusion matrix
- Built a small "Virtual A&R Simulator" that predicts the probability of a new song becoming a hit

## Dataset

The dataset is too large to upload to GitHub.

You can download it here:

https://drive.google.com/uc?export=download&id=1sD9s9pHsc2EO230RGoVD7hpJ0_6IoRab

After downloading, place the CSV file in the project directory (or update the path in the notebook).

## Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Seaborn
- SciPy

## Results

The final model achieved roughly **80% training accuracy** and **78% validation accuracy**.

One of the more interesting parts of the project was comparing a model trained on only 5% of the data with one trained on the full dataset. The larger dataset produced more stable learning and better validation performance, even though the improvement was smaller than I initially expected.
