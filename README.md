# Housing Price Prediction using Linear Regression

This project demonstrates Linear Regression from scratch (using Gradient Descent) to predict housing prices based on the Kaggle Housing Prices Dataset.
The implementation is done in Google Colab with complete data preprocessing, training, and evaluation.

# Dataset

Dataset: Housing Prices Dataset (Kaggle)

File: Housing.csv

Features:

area → Size of the house (sq. ft)

price → Price of the house (target variable)

# Project Workflow
1. Setup Kaggle in Colab
!pip install kaggle -q
from google.colab import files
files.upload()  # Upload kaggle.json
!mkdir -p ~/.kaggle && mv kaggle.json ~/.kaggle/ && chmod 600 ~/.kaggle/kaggle.json

2. Download & Extract Dataset
!kaggle datasets download -d yasserh/housing-prices-dataset
!unzip -o housing-prices-dataset.zip

3. Data Preprocessing

Load data using pandas.

Select area as input feature (X) and price as target (y).

Train-test split (80:20).

Standardize features using StandardScaler.

4. Implement Linear Regression (Gradient Descent)

Initialize slope m and intercept c.

Update parameters iteratively using Gradient Descent.

Track R² Score (accuracy).

5. Visualization

Plot Epoch vs Accuracy (R² Score).

# Results

The model learns the relationship between area and price.

Accuracy improves across epochs.

Final output includes:

Slope (m)

Intercept (c)

Train R² Score

Test R² Score
