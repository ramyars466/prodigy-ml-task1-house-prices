# Prodigy ML Task 01 – House Price Prediction

This repository contains my solution for **Task 01** of the Prodigy InfoTech Machine Learning internship.

The goal is to build a **linear regression model** to predict house prices using the
[Kaggle House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset.[web:12]

## Features and Target

- `GrLivArea` – Above-ground living area (square feet)
- `BedroomAbvGr` – Number of bedrooms above ground
- `FullBath` – Number of full bathrooms
- Target: `SalePrice`

## Approach

1. Loaded `train.csv` and `test.csv` from the Kaggle competition.
2. Selected the three required numerical features and handled missing values using median imputation.
3. Trained a baseline **LinearRegression** model and evaluated it with **RMSE** and **R²**.
4. Improved performance by adding **PolynomialFeatures** and tuning the polynomial degree with **GridSearchCV**, keeping the model in the linear regression family.[web:66][web:81]
5. Trained the best model on all training data and generated predictions for the Kaggle test set.

## Files

- `house_price_prediction_task1.ipynb` – main Colab notebook (click the badge to open in Colab).
- `README.md` – overview of the project.

## How to run

1. Open the notebook in Google Colab using the "Open in Colab" button.
2. Upload `train.csv` and `test.csv` from the Kaggle competition.
3. Run all cells to reproduce the results.
4. 
## Outputs

- `submission.csv` – model predictions (`Id`, `SalePrice`) for all rows in `test.csv`.
- The notebook also displays a preview of the predicted prices using `submission.head()`.
