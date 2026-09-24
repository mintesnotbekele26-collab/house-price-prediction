# House Price Prediction

## Project Overview

This project predicts house prices using **Linear Regression**. Three models were developed and compared:

1. **Univariate Linear Regression** — uses `area`
2. **Bivariate Linear Regression** — uses `area` and `bathrooms`
3. **Multivariate Linear Regression** — uses multiple house features

The goal is to understand how adding more relevant features affects house price prediction performance.

## Dataset

The project uses the Housing.csv dataset, which contains information about houses and their prices.

The dataset includes numerical and categorical features such as:

* Area
* Bedrooms
* Bathrooms
* Stories
* Parking
* Main road
* Guest room
* Basement
* Hot water heating
* Air conditioning
* Preferred area
* Furnishing status
* Price

## Models

### 1. Univariate Linear Regression

Uses only **area** to predict house price.

**R²:** 0.273

### 2. Bivariate Linear Regression

Uses **area** and **bathrooms** to predict house price.

**R²:** 0.429

### 3. Multivariate Linear Regression

Uses multiple features to predict house price.

**R²:** 0.649

## Model Comparison

| Model        |       MAE |      RMSE |    R² |
| ------------ | --------: | --------: | ----: |
| Univariate   | 1,474,748 | 1,917,104 | 0.273 |
| Bivariate    | 1,295,658 | 1,698,621 | 0.429 |
| Multivariate |   979,680 | 1,331,071 | 0.649 |

The models were evaluated using **MAE, MSE, RMSE, and R²**.

## Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Structure


house-price-prediction/
│
├── notebooks/
│   └── house_price_prediction.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore


## Conclusion

The multivariate Linear Regression model achieved the highest R² among the three models tested, showing that using multiple house features improved prediction performance compared with using only one or two features.
