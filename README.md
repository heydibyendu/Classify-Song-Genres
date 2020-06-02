# Classify Song Genres

Streaming services categorize music to allow for personalized recommendations. They directly analyze the raw audio information and score the raw data on a variety of metrics. With this project, I have analyzed music steaming data compiled by a music intelligence and data platform known as '[The Echo Nest](https://en.wikipedia.org/wiki/The_Echo_Nest),' now part of Spotify.

## Goal
The goal of the project was to look through the dataset and classify the genre of a song and that too without listening to music.

## Dataset
The music steaming data is composed of two datasets: the first dataset is about the tracks alongside the track metrics, and the second dataset is about the musical features on a scale from -1 to 1. The two datasets are concatenated, and this is how the first 5 rows of the dataset look like:

![Image](https://github.com/heydibyendu/Classify-Song-Genres/blob/master/dataset_head.png)

## Modelling
I trained Logistic Regression as my baseline model and then added KNN, SVM and Random Forest. Unsurprisingly, Random Forest turned out to be the best model in the pack, leaving behind Logistic Regression by more than 3 percentage points in accuracy.

## Results
The model achieved 84.95% accuracy in predicting genres through parameter estimation in the training set. I used grid search with 10-fold cross-validation for tuning the parameters. In the held-out validation set, the model achieved an accuracy of 84.59%, which matches closely to the expectations estimated during the tuning of Random Forest.

## Lessons
This project taught me about how to manipulate data, including handling outliers as well as dimensionality reduction, prepare the dataset for model building, and build a robust machine learning model.
