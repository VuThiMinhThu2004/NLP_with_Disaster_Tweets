# Natural Language Processing with Disaster Tweets - Classification Using BERT

## Overview

This project implements a disaster tweet classification system using **BERT (Bidirectional Encoder Representations from Transformers)**, a state-of-the-art natural language processing model. The goal is to determine whether a given tweet is about a disaster or not. This solution is built on the Kaggle competition dataset: *NLP with Disaster Tweets*.

---

## Features

- **Text Preprocessing**: Comprehensive cleaning of tweets, including:
  - Expanding contractions (e.g., `can't -> cannot`).
  - Removing URLs, emojis, HTML tags, and punctuation.
  - Standardizing abbreviations and converting words to a basic form (lemmatization).
  
- **Feature Engineering**:
  - Tokenization and attention mask creation using BERT tokenizer.
  - Conversion of tweets to numerical representations for input to BERT.

- **Model Training**:
  - Fine-tuning of **BERT-large-uncased** with a classification head for binary classification.
  - Utilization of **AdamW optimizer** with a linear learning rate scheduler for optimal convergence.
  
- **Evaluation**:
  - Performance metrics: **Accuracy**, **F1 Score**, and **Loss** on the validation set.
  - Epoch-wise training and testing statistics with graphical visualization.

- **Prediction**:
  - Classifies unseen tweets into disaster or non-disaster categories.
  - Outputs a submission file in the required format for Kaggle.

---

## Dataset

The dataset consists of:
1. `train.csv`: Training data with labeled tweets.
2. `test.csv`: Unlabeled test data for predictions.
3. `sample_submission.csv`: Template for submission.

---
## How to Use

### Train the Model
- Run the notebook to preprocess data, fine-tune BERT, and evaluate the model.

### Generate Predictions
- Once training is complete, the script predicts the labels for the test dataset and saves the results in `submission.csv`.

### Submit to Kaggle
- Upload `submission.csv` to Kaggle to evaluate the model's performance.

---

## Dependencies

- **Python 3**

- **Libraries**:
  - `transformers`
  - `torch`
  - `tensorflow`
  - `nltk`
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`

---
.

