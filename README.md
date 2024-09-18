# Sales Forecasting Project for Rossmann sales data

## Overview
Rossmann operates over 3,000 drug stores across 7 European countries. Store managers are tasked with predicting daily sales up to six weeks in advance. Sales are influenced by various factors including promotions, competition, holidays, seasonality, and locality. This project aims to enhance sales prediction accuracy through advanced data analysis and machine learning techniques.

## Data Files
- **Rossmann Data**: Contains information about each store.
- **store.csv**: Holds daily sales information for each store.

## Business Problem
Store managers face challenges in accurately predicting sales due to varying influences across different stores and regions. The goal is to develop a model that can accurately forecast sales on a given day by analyzing historical data and key factors affecting sales.

## Steps for Solving the Business Problem

### 1. Collecting Data
- Upload and explore the .csv files using methods like `.head()`, `.info()`, and `.describe()` to understand the structure and contents of the data.

### 2. Preparing the Data
- Clean the data by removing unwanted entries, handling missing values, correcting data types, and visualizing relationships between variables.
- Split the data into training and testing sets: the training set is used for model training and parameter optimization, while the testing set evaluates the model’s accuracy.

### 3. Choosing and Training the Model
- Implement and train various machine learning models, including Decision Tree, Regression, Random Forest, Elastic Net, Lasso, Ridge, AdaBoost, and XGBoost.

### 4. Hyperparameter Tuning
- Optimize model performance through careful tuning of hyperparameters to enhance accuracy and prevent overfitting.

### 5. Making Predictions
- Generate predictions and evaluate model performance using metrics such as RMSE, accuracy, and RMPSE.

## Results and Conclusion
- **Sales Column Analysis**: Initially, we removed rows with 0 sales, which led to an accuracy of around 74%.
- **Full Dataset Analysis**: Including all rows, even those with 0 sales, resulted in an improved accuracy of approximately 98%.
- **Conclusion**: Removing rows with 0 sales resulted in the loss of significant information. Therefore, including these rows in the dataset is crucial for better model performance. The Random Forest, Gradient Boosting (e.g., AdaBoost), and XGBoost models provided the best results, with careful parameter tuning to avoid overfitting.

## Key Models
- **XGBoost**: Effective for classification and regression with techniques such as SMOTE oversampling and scale_pos_weight adjustment.
- **Decision Tree**: Provides insights into feature importance and decision-making rules.
- **Regression**: Used for baseline performance and understanding variable relationships.
- **Random Forest**: Enhances accuracy by combining multiple decision trees.
- **Elastic Net**: Balances feature selection and regularization.
- **Lasso and Ridge**: Manage multicollinearity and perform feature selection.
- **AdaBoost**: Boosting technique to improve prediction performance.
- **SARIMAX**: Time series forecasting with seasonal components.

## Model Interpretability
- **SHAP (SHapley Additive exPlanations)**: Offers insights into the impact of each feature on model predictions.
- **LIME (Local Interpretable Model-agnostic Explanations)**: Provides explanations for individual predictions.

## Installation
Clone the repository and install the necessary packages:

```bash
[git clone https://github.com/VENKATAGOPI3341/Sales-Forecasting-ml-techniques.git]
cd Sales-Forecasting-ml-techniques
pip install -r requirements.txt
