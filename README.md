# Business Revenue Regression

A machine learning project focused on predicting **annual business revenue** using regression models and feature preprocessing techniques.

## 📌 Project Overview

The goal of this project is to predict a company's annual revenue based on various business and demographic features.

The dataset contains **1,200 observations** and includes numerical and categorical features such as:

* Age
* Experience years
* Monthly advertising spend
* Website visits
* Team size
* Customer rating
* Region
* Business type
* Subscription plan
* Additional numerical features

The target variable is:

**`annual_revenue`**

The dataset is loaded from https://www.kaggle.com/datasets/abdallahwagih/business-revenue-regression-dataset/data

## 🔍 Exploratory Data Analysis

The dataset was initially explored using:

* `head()`
* `info()`
* `describe()`
* Correlation analysis
* Correlation heatmap

Categorical features were also examined before applying preprocessing techniques.

## ⚙️ Data Preprocessing

The following preprocessing steps were applied:

1. Separation of features and target variable
2. Train-test split
3. One-Hot Encoding for categorical variables
4. Feature scaling using `StandardScaler`

The categorical variables included:

* `region`
* `business_type`
* `subscription_plan`

`OneHotEncoder` was configured with `handle_unknown='ignore'` to handle previously unseen categories.

## 🤖 Models

Several regression models were implemented and compared:

* Linear Regression
* Lasso Regression
* Ridge Regression
* ElasticNet Regression

## 📊 Evaluation Metrics

The models were evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score
* Adjusted R² Score

### Results

| Model             | R² Score | Adjusted R² |
| ----------------- | -------: | ----------: |
| Linear Regression |   0.8527 |      0.8449 |
| Lasso Regression  |   0.8527 |      0.8449 |
| Ridge Regression  |   0.8529 |      0.8451 |
| ElasticNet        |   0.7810 |      0.7695 |

The results are based on the train-test split and preprocessing implemented in the notebook.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## 📁 Project Structure

```text
BusinessRevenueRegressions/
│
├── Annual_Revenue.ipynb
├── dataset.csv
└── README.md
```

## 📚 What I Practiced

Through this project, I practiced:

* Exploratory Data Analysis
* Feature-target separation
* Train-test splitting
* Categorical feature encoding
* Feature scaling
* Linear Regression
* Regularization with Lasso and Ridge
* ElasticNet Regression
* Regression model evaluation
* Comparing different regression approaches
