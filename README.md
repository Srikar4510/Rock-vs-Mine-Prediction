# Rock vs Mine Prediction

This project aims to classify objects as either rocks or mines using sonar data and a logistic regression model. The dataset used contains 60 features per instance, representing sonar returns bounced off different surfaces.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Data Processing](#data-processing)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Making Predictions](#making-predictions)
- [Results](#results)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In this project, we leverage machine learning techniques to classify sonar data into two categories: rocks and mines. By training a logistic regression model on labeled sonar data, we aim to predict the category of new instances accurately.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Rock-vs-Mine-Prediction.git
    cd Rock-vs-Mine-Prediction
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Dataset

The dataset used in this project is the Sonar dataset, which contains 208 instances with 60 attributes each. The attributes are numerical values representing the energy within a particular frequency band.

- **File**: `sonar_data.csv`
- **Attributes**: 60 numeric values
- **Labels**: `M` (Mine) or `R` (Rock)

## Data Processing

1. Load the dataset into a pandas DataFrame.
2. Explore the dataset: view the first few rows, check the shape, generate descriptive statistics, and check for missing values.
3. Separate the features and labels.

## Model Training

1. Split the dataset into training and testing sets using `train_test_split` from scikit-learn.
2. Train a Logistic Regression model on the training data.

## Model Evaluation

1. Predict the labels for the training data and calculate the accuracy.
2. Predict the labels for the test data and calculate the accuracy.

## Making Predictions

1. Define the input data for prediction.
2. Convert the input data to a numpy array and reshape it for prediction.
3. Use the trained model to predict the label.
4. Output whether the object is a rock or a mine.

## Results

- **Accuracy on training data**: 83.42%
- **Accuracy on test data**: 76.19%

