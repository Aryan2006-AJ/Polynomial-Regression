# Polynomial Regression – Medical Cost Prediction

## 📌 Project Overview

This project implements Polynomial Regression in Python to predict medical insurance charges using the Medical Cost Personal Dataset.

The main objective is to study the relationship between BMI and medical insurance charges and compare Linear Regression with Polynomial Regression models of different degrees.

## 🎯 Objectives

- Load and explore the Medical Cost Personal Dataset.
- Analyze the relationship between BMI and medical charges.
- Split the dataset into training and testing sets.
- Implement Linear Regression as a baseline model.
- Implement Polynomial Regression for degrees 2 to 5.
- Compare different polynomial degrees using evaluation metrics.
- Predict medical charges for a new BMI value.
- Visualize the regression curves.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 📂 Dataset

The project uses the `insurance.csv` Medical Cost Personal Dataset.

The main variables used for the original experiment are:

- **BMI** – Independent Variable
- **Charges** – Dependent Variable

## ⚙️ Methodology

1. Imported the required Python libraries.
2. Loaded the `insurance.csv` dataset.
3. Inspected the dataset structure, data types, and statistics.
4. Selected BMI as the independent variable and charges as the dependent variable.
5. Visualized BMI against medical charges.
6. Split the data into training and testing sets using an 80:20 ratio.
7. Built a Linear Regression baseline model.
8. Created Polynomial Regression models with degrees 2, 3, 4, and 5.
9. Evaluated each model using:
   - R² Score
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
10. Compared the performance of all models.
11. Predicted medical charges for a new BMI value.
12. Visualized the polynomial regression curves.

## 📊 Model Comparison

For the BMI-based experiment, the models produced the following test results:

| Degree | R² Score | RMSE |
|-------:|---------:|-----:|
| 1 | 0.0397 | 12210.04 |
| 2 | 0.0308 | 12266.73 |
| 3 | 0.0180 | 12347.17 |
| 4 | 0.0146 | 12368.61 |
| 5 | 0.0130 | 12378.67 |

### Best Model

Based on the test R² score and RMSE among the tested degrees:

**Best Degree: 1**

**R² Score: 0.0397**

**R² Percentage: 3.97%**

This experiment shows that increasing the polynomial degree did not improve the test performance for predicting charges from BMI alone.

> Note: R² Score is a regression evaluation metric and should not be interpreted as classification accuracy.

## 📈 Additional Experiment – Age

An additional experiment was also performed using **Age** as the independent variable and **Charges** as the dependent variable.

Polynomial Regression models of different degrees were compared to study whether age provides a stronger relationship with medical charges.

