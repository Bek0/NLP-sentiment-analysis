# README for NLP and Sentiment Analysis Project

## Overview

This project focuses on sentiment analysis of textual comments using natural language processing (NLP) and machine learning techniques. The primary objective is to classify sentiments from text data, identify key phrases, and analyze various metrics related to sentiment and text content.

## Data Preprocessing

- **Data Loading**: The dataset is loaded from a CSV file containing textual comments along with sentiment scores and numerical scores.
  
- **Text Cleaning**:
  - **HTML and URL Removal**: HTML entities and URLs are stripped from the text to remove irrelevant content and potential noise.
  - **Normalization**: Text is converted to lowercase to ensure uniformity.
  - **Punctuation and Special Characters Removal**: All punctuation, special characters, and digits are removed to clean the text and focus on meaningful words.
  - **Whitespace Handling**: Multiple whitespace characters are replaced with a single space for better text processing.

- **Tokenization and Lemmatization**:
  - **Tokenization**: Text is split into individual words or tokens.
  - **Stop Words Removal**: Common stop words (e.g., "and", "the") are removed to focus on significant words.
  - **Lemmatization**: Words are reduced to their base or root form to standardize variations of words.

## Feature Extraction

- **TF-IDF Vectorization**:
  - **Term Frequency-Inverse Document Frequency (TF-IDF)**: This technique transforms text data into numerical features that represent the importance of each word in relation to the entire dataset.
  - **Feature Selection**: Selected the top features based on their significance to enhance model performance.

## Data Analysis

- **Sentiment Distribution**:
  - Analyzed the distribution of sentiments across the dataset to understand the overall sentiment landscape.
  
- **Comment Length Analysis**:
  - Examined the average length of comments by sentiment class to identify any trends or patterns related to comment length.

- **Score Analysis**:
  - **Sentiment Scores**: Investigated the distribution of numerical scores associated with each sentiment class.
  - **Average Scores**: Computed the average scores for positive and negative comments to assess their intensity.

- **Keyword and Word Frequency**:
  - **Top Keywords**: Identified the most frequently mentioned keywords and phrases in the comments.
  - **Word Frequency**: Analyzed the frequency of words to uncover common themes or topics.

## Model Training and Evaluation

- **Data Splitting**:
  - Divided the dataset into training and testing sets to evaluate model performance on unseen data.

- **Model Construction**:
  - **Feature Extraction Pipeline**: Built a pipeline that combines TF-IDF vectorization and feature selection.
  - **Ensemble Classification**: Used an ensemble model comprising Logistic Regression and AdaBoost to classify sentiments.

- **Training**:
  - Trained the model on the training dataset to learn patterns and make predictions.

- **Evaluation**:
  - **Confusion Matrix**: Evaluated model performance by computing a confusion matrix to visualize the true vs. predicted classifications.
  - **Classification Report**: Generated a detailed classification report including metrics such as precision, recall, and F1-score to assess model accuracy and effectiveness.
