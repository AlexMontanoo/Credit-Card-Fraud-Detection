# Credit Card Fraud Detection

## Project Overview

This project involves building a machine learning model to detect fraudulent credit card transactions. The dataset contains anonymized transaction data, with features describing transaction details and a binary target variable indicating whether the transaction was fraudulent (`Class` column: 1 for fraud, 0 for genuine). The goal is to create a classification model that can predict fraudulent transactions with high accuracy.

## Problem Statement

Credit card fraud is a major concern for financial institutions and their customers. Fraud detection systems must be able to identify fraudulent transactions quickly to minimize losses. Given a dataset of credit card transactions, the task is to classify each transaction as either fraudulent or legitimate. Since fraudulent transactions are much less frequent, the dataset is highly imbalanced, presenting challenges in training an accurate model.

## Steps Involved

1. **Data Preprocessing**:
   - Load the dataset and examine the features.
   - Handle missing values (if any).
   - Split the data into training and testing sets.
   - Normalize/standardize features, if necessary, to improve model performance.

2. **Model Selection**:
   - A **Random Forest Classifier** was chosen due to its ability to handle imbalanced datasets, and its effectiveness in classification tasks.

3. **Model Training**:
   - Train the Random Forest model on the training dataset.
   - Fine-tune the hyperparameters to optimize performance.

4. **Model Evaluation**:
   - Evaluate the model using metrics such as **F1 Score** and **Confusion Matrix** to measure its effectiveness at detecting fraudulent transactions.
   - Since the dataset is highly imbalanced, the F1 score is particularly useful to balance precision and recall.

## Evaluation Metrics

- **Confusion Matrix**: Shows the number of true positives, false positives, true negatives, and false negatives.
- **F1 Score**: The harmonic mean of precision and recall. F1 score is particularly useful for imbalanced datasets as it considers both false positives and false negatives.

## Results

The Random Forest model achieved an F1 score of **0.86**, indicating a good balance between precision and recall. The confusion matrix revealed that the model was able to correctly identify a significant number of fraudulent transactions.

## Technologies Used

- **Python**: The programming language used for data processing and model development.
- **Libraries**:
  - `pandas`: Data manipulation and analysis.
  - `numpy`: Numerical operations.
  - `XGBoost` (or any other library used): Machine learning model for classification.
  - `matplotlib` / `seaborn`: Data visualization.

