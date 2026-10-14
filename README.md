# Classical ML and Honest Evaluation

This repository contains my Week 2 internship work, focused on classical machine learning, model validation, preventing data leakage, and evaluating model generalization performance.

## Overview

The work in this project covers both:

- Classification problems, using customer churn prediction as the main example.
- Regression problems, using stock price forecasting as the second example.

Across the project, key concepts are introduced and applied, including:

- Supervised learning
- Train/validation/test splits
- Cross-validation
- Feature encoding and preprocessing
- Model comparison
- Overfitting and underfitting
- Honest evaluation and data leakage prevention
- Time-series-aware validation for forecasting tasks


## Day 1: Customer Churn Prediction

The first project focuses on a binary classification problem: predicting whether a customer is likely to churn.

### What was covered

- Exploring the telco customer dataset
- Defining the target variable (`Churn`)
- Cleaning and preparing the dataset
- Handling categorical data with encoding techniques
- Splitting data into train and test sets
- Training baseline models such as logistic regression
- Evaluating model performance using metrics like accuracy, precision, recall, F1-score, and ROC-AUC
- Understanding class imbalance and generalisation

### Tools and techniques used

- Python
- pandas
- scikit-learn
- Jupyter Notebook

## Day 2: Honest Evaluation and Model Checking

This day focuses on the idea that model performance must be measured honestly. The emphasis is on evaluating how models behave on unseen data without accidentally leaking information from the future or from the test set into training.

### What was covered

- The difference between training, validation, and test data
- Why random splits are not always appropriate
- The risk of data leakage
- Overfitting versus underfitting
- Cross-validation and stratified cross-validation
- Baseline comparison across multiple models
- Model selection based on realistic evaluation rather than training scores alone

### Main learning goal

Build the habit of assessing models in a way that reflects real-world performance and avoids misleadingly optimistic results.

## Day 3: Stock Price Prediction

The third project shifts from classification to regression, using historical stock market data to predict the next day’s closing price for Apple stock.

### What was covered

- Working with market time-series data
- Selecting a single stock (AAPL)
- Creating a target variable (`Tomorrow_Close`)
- Handling time ordering carefully to avoid leakage
- Training regression models on historical data
- Comparing model performance using honest validation strategies
- Understanding why time-series forecasting needs special handling


## Tech Stack

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn

## Getting Started

1. Clone the repository.
2. Open the notebook in the relevant day folder using Jupyter or VS Code.
3. Install the required Python packages if needed:

```bash
pip install pandas numpy scikit-learn notebook
```

4. Run the notebooks in order to follow the progression from raw data to model evaluation.

## Notes

This project is educational and exploratory. It demonstrates classical machine learning workflows and evaluation principles rather than production-ready deployment code.

## Learning Outcomes

By the end of this project, the main skills developed include:

- Cleaning and preparing real-world datasets
- Building machine learning workflows from start to finish
- Encoding categorical features correctly
- Comparing classical models
- Applying honest evaluation strategies
- Identifying overfitting, underfitting, and leakage
- Interpreting model performance with careful judgement

