# Quora-Duplicate-Question-Pairs

## Overview
This project aims to develop a machine learning model that can identify duplicate questions on Quora.The goal is to reduce redundancy and improve the overall quality of Quora content by identifying and merging duplicate questions.


The project uses a dataset of Quora question pairs, where each pair is labeled as either a duplicate or not a duplicate. The dataset was collected by Quora and made publicly available on Kaggle. The dataset contains over 400,000 question pairs, which are split into a training set and a test set.

## Methodology 

The project involves several steps, including data cleaning and preprocessing, feature extraction, model selection and training, and model evaluation.

## Data Cleaning and Preprocessing

The data cleaning and preprocessing step involves removing any unwanted characters or punctuation, converting all text to lowercase, and removing stop words. In addition, Bag of Words is used to preprocess the Quora question pairs and create a feature set that can be used for training the model.

## Feature Extraction

The feature extraction step involves converting the preprocessed text data into a numeric representation that can be used as input to a machine learning model. In this project, custom feature engineering is used to capture additional information that may be relevant to the classification task. These features include the following:

* Bag of Words: The preprocessed text is converted to a numeric vector representation using the Bag of Words technique.
* Fuzzy Wuzzy: String similarity measures are calculated between the preprocessed question pairs using the Fuzzy Wuzzy library. Metrics such as Levenshtein distance, Jaro distance, and cosine similarity are used to calculate these similarity measures, which are then added as features to the dataset.

## Model Selection and Training

The model selection and training step involves selecting an appropriate machine learning algorithm and training it on the preprocessed and feature-engineered data. In this project, Random Forest is used for classification of the Quora question pairs. The algorithm can handle high-dimensional feature sets and has been shown to perform well on text classification tasks.

## Model Evaluation

The model evaluation step involves evaluating the accuracy of the trained model on a separate test set of Quora question pairs. The performance of the model is measured using metrics such as accuracy and Confusion Matrix.

# Dependencies

The project uses the following libraries and tools:

* Python 3.6+
* pandas
* NumPy
* scikit-learn
* NLTK
* Fuzzy Wuzzy
