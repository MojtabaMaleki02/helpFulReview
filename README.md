# Helpful Review Predictor

The Helpful Review Predictor is a Python package that predicts the helpfulness of reviews using machine learning techniques. It takes textual reviews as input and provides a binary classification indicating whether the review is likely to be helpful or not. if the output is 1, then the review is helpful. But if the output is 0, it means that the review is not helpful.

## Features

- Preprocesses textual reviews, including lowercasing, punctuation removal, contractions expansion, and lemmatization.
- Uses TF-IDF vectorization to convert text data into numerical feature vectors.
- Handles class imbalance using Random Over Sampling.
- Supports training and evaluation of multiple classifiers, including Gaussian Naive Bayes, Logistic Regression, and Decision Trees.
- Performs hyperparameter tuning using Grid Search and Stratified K-Fold Cross Validation.
- Provides visualization tools for comparing different classifiers and evaluating model performance.
- Saves the best model and TF-IDF vectorizer for future use.

## Installation

You can install the Helpful Review Predictor package using pip:

```bash
pip install helpful-review-predictor
```

## Usage

```python
from helpful_review_predictor import predict_helpfulness

review = "I purchased this product a few weeks ago and have been thoroughly impressed with its performance..."
prediction = predict_helpfulness(review)
print("Predicted helpfulness:", prediction)
```

## Requirements
+ scikit-learn
+ numpy
+ scipy
+ joblib
+ textblob
+ nltk
+ imbalanced-learn
