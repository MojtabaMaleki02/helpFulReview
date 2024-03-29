# Helpful Review Predictor

The Helpful Review Predictor is a Python package that predicts the helpfulness of reviews using machine learning techniques. It takes textual reviews as input and provides a binary classification indicating whether the review is likely to be helpful or not. A prediction of 1 indicates a helpful review, while a prediction of 0 indicates a review that is not helpful.

For a comprehensive understanding of the model's training process and methodology, I have documented it in an academic research paper. To stay updated on the latest developments and access the research paper upon publication, I invite you to follow my LinkedIn profile: [Mojtaba Maleki](https://www.linkedin.com/in/mojtabamaleki02/).

## Dataset

The data used for training the model is sourced from the Amazon Electronics Reviews dataset available on Kaggle. This 5-core dataset contains product reviews from the Electronics category on Amazon from May 1996 to July 2014, totaling 1,689,188 entries.

The dataset is provided by Julian McAuley, UCSD, and is available [here](http://jmcauley.ucsd.edu/data/amazon/).

## Features

- Preprocesses textual reviews, including lowercasing, punctuation removal, contractions expansion, and lemmatization.
- Utilizes TF-IDF vectorization to convert text data into numerical feature vectors.
- Addresses class imbalance using Random Over Sampling.
- Supports training and evaluation of multiple classifiers, including Gaussian Naive Bayes, Logistic Regression, and Decision Trees.
- Performs hyperparameter tuning using Grid Search and Stratified K-Fold Cross Validation.
- Provides visualization tools for comparing different classifiers and evaluating model performance.
- Saves the best model and TF-IDF vectorizer for future use.

## Installation

You can install the Helpful Review Predictor package using pip:

```bash
pip install helpful-review-predictor
```

### Usage

```python
from helpfulReviewPredictor import PredictHelpfulness

string_input = "Your input string here"
predictor = PredictHelpfulness(string_input)
result = predictor.get_result()
print(result)  # Output: 1 for Helpful, 0 for Not Helpful
```

### Requirements

- joblib
- numpy
- scikit-learn
- scipy
- TfidfVectorizer from sklearn.feature_extraction.text


These changes provide more clarity about the purpose of the package, the dataset used, and the expected output. They also improve the formatting and readability of the document.
