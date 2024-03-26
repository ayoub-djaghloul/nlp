# TP2: Sentiment Analysis with SVM

## Auteur
DJAGHLOUL AYOUB AHMED AMINE

## Overview
This project involves the implementation of a Support Vector Machine (SVM) classifier for sentiment analysis on Twitter data. The objective is to classify tweets into positive, negative, or neutral categories based on their content.

## Environment Setup
Ensure you have Python 3.6+ installed along with the following packages:
- pandas
- scikit-learn
- re (regular expressions)

### Installing Dependencies
Install the required Python packages using pip:

```bash
pip install pandas scikit-learn
```

## Data Preprocessing
Data is loaded from text files containing tweets with their sentiment labels. Text preprocessing steps include converting text to lowercase, removing non-word characters, and replacing multiple spaces with a single space.

### Load Data
The datasets used are `twitter-2013train-A.txt`, `twitter-2013dev-A.txt`, and `twitter-2013test-A.txt`, containing training, development, and test data respectively.

## Feature Extraction
A unique numerical identifier is assigned to each word in the dataset's lexicon. Tweet texts are then converted into feature vectors based on word occurrences.

## SVM Classification
An SVM model is trained on the processed data. This model is then used to predict the sentiment of tweets in the development and test sets.

### Model Evaluation
The model's performance is evaluated using precision, recall, and F1-score metrics, with results detailed for each sentiment category.

## Results
The results section includes classification reports for both the development and test datasets, highlighting the effectiveness of the SVM classifier in sentiment analysis tasks.
