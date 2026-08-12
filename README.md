# Used Bike Price Prediction using K-Nearest Neighbors (KNN)

## Project Overview

This project focuses on building a Machine Learning model to predict the prices of used bikes using the K-Nearest Neighbors (KNN) algorithm.

The model uses important features such as bike power, owner's age, and kilometers driven to estimate the selling price of a used bike. The objective is to help buyers and sellers make better pricing decisions.

## Objectives

- Predict the price of used bikes using Machine Learning.
- Perform Exploratory Data Analysis (EDA).
- Identify important features affecting bike prices.
- Apply data preprocessing techniques.
- Build a KNN regression model.
- Evaluate the model using K-Fold Cross-Validation.
- Compare KNN performance with Linear Regression.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand the dataset and identify important patterns and relationships.

The analysis included:

- Checking the dataset structure and data types
- Handling missing values
- Statistical analysis
- Distribution analysis
- Data visualization
- Identifying relationships between features and bike prices

## Feature Selection

Important features were selected based on their relevance to bike prices.

### Input Features

- Power
- Owner Age
- Kilometers Driven

### Target Variable

- Price

## Label Encoding

Categorical variables were converted into numerical values using Label Encoding so that they could be processed by the Machine Learning algorithm.

## Correlation Analysis

Pearson Correlation Analysis was performed to measure the strength and direction of the relationship between the input features and the target variable.

This analysis helped identify which features have a stronger relationship with bike prices.

## Machine Learning Model

### K-Nearest Neighbors (KNN)

The K-Nearest Neighbors regression algorithm was used to predict used bike prices.

KNN predicts the price of a bike by identifying the most similar bikes in the training dataset and using their prices to estimate the price of a new bike.

## K-Fold Cross-Validation

K-Fold Cross-Validation was used to evaluate the model more reliably.

The dataset was divided into multiple subsets called folds. The model was trained on some folds and validated on the remaining fold. This process was repeated multiple times, with each fold being used as the validation set.

This provided a more reliable estimate of the model's performance.

## Results

The initial Linear Regression model achieved approximately 65% performance.

After implementing the KNN algorithm and applying K-Fold Cross-Validation, the model achieved approximately 93% performance.

| Model | Performance |
|---|---:|
| Linear Regression | ~65% |
| KNN Regression + K-Fold Cross-Validation | ~93% |

The results demonstrate that KNN performed significantly better than the initial Linear Regression model for this dataset.

Note: Since this is a regression problem, metrics such as R-squared (R2), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE) are more appropriate than classification accuracy.

## Key Insights

- Used bike prices are influenced by multiple factors.
- Power and kilometers driven are important factors for price prediction.
- Feature selection can improve model performance.
- KNN performed better than the initial Linear Regression model.
- K-Fold Cross-Validation provides a more reliable evaluation of the model.

## Project Structure

```text
Used-Bike-Price-Prediction/
|
|-- dataset/
|   |-- used_bikes.csv
|
|-- notebook/
|   |-- Used_Bike_Price_Prediction.ipynb
|
|-- README.md
|-- requirements.txt
