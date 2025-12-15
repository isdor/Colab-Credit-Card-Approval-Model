# Colab Credit Card Approval Model

This repository contains a Google Colab notebook that demonstrates the implementation of a logistic regression model to predict credit card approval status.

## Project Overview

The goal of this project is to build a machine learning model that can determine if an individual's credit card application will be accepted. The notebook covers the entire machine learning pipeline, from data loading and cleaning to model evaluation.

## Dataset

The project uses the [Credit Card Approval dataset](http://archive.ics.uci.edu/ml/datasets/credit+approval) from the UCI Machine Learning Repository. Due to confidentiality, the feature names are anonymised.

## Key Steps

1.  **Data Loading and Initial Exploration**: Loading the dataset and performing an initial review of its structure and content.
2.  **Data Cleaning**: Handling missing values by replacing '?' with NaN, imputing numeric columns with their mean, and non-numeric columns with their mode.
3.  **Data Preprocessing**: 
    *   Converting non-numeric data into numeric using `LabelEncoder`.
    *   Dropping irrelevant features.
    *   Splitting data into features (X) and labels (y).
    *   Standardising features using `MinMaxScaler`.
    *   Splitting data into training and testing sets (80/20 split) with `random_state=42`.
4.  **Model Training**: Training a Logistic Regression model using `sklearn.linear_model.LogisticRegression` with the 'lbfgs' solver.
5.  **Model Evaluation**: Assessing the model's performance using:
    *   AUC-ROC score
    *   Accuracy
    *   Precision
    *   Recall
    *   F1-score

## How to Use

1.  Open the `credit_card_approval_model.ipynb` notebook in Google Colab.
2.  Run the cells sequentially to follow the data processing, model training, and evaluation steps.
3.  Modify the code as needed for further experimentation or to apply to different datasets.

## Requirements

This notebook uses standard Python libraries, which are typically pre-installed in Google Colab or can be installed via `pip`:

*   `numpy`
*   `pandas`
*   `scikit-learn`

## Author

*   **Explore-AI Academy** (Original Challenge Provider)
*   **Isdor Otieno** 
