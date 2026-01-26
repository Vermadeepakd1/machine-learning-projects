# 📌 Project: House Price Prediction

## Problem

Predict house prices using regression models.

## Dataset

Source: [Kaggle - Home Value Insights](https://www.kaggle.com/datasets/prokshitha/home-value-insights)
Brief description: 1000 houses with features: Num_Bedrooms, Num_Bathrooms, Garage_Size, Square_Footage, Year_Built, Lot_Size, Neighborhood_Quality, and House_Price (target). The goal is to predict House_Price using these features. The dataset is clean, with minimal missing values and no duplicates.

## Steps Performed

- EDA
- Cleaning
- Feature encoding
- Scaling
- Model training
- Evaluation

## Models Used

- Linear Regression
- Ridge
- Lasso

## Results

- Best R² (Linear Regression): 0.89
- Best R² (Ridge): 0.88
- Best R² (Lasso): 0.87
- Best RMSE (Linear Regression): 32,000
- Best RMSE (Ridge): 33,000
- Best RMSE (Lasso): 34,000
- DummyRegressor RMSE (baseline): 95,000

## Key Learnings

- The most important feature for predicting house price was **Square_Footage**, followed by **Neighborhood_Quality** and **Lot_Size**.
- Scaling the features (StandardScaler) improved model convergence and performance.
- Regularization (Ridge, Lasso) reduced the magnitude of coefficients and helped prevent overfitting, but Linear Regression performed best on this dataset.
- DummyRegressor baseline shows the value of using real models: RMSE dropped from 95,000 (dummy) to 32,000 (linear regression).

### 🧪 Experiments

**Experiments performed and suggested:**

- Compared model performance with and without feature scaling (StandardScaler). Scaling improved convergence and model accuracy.
- Analyzed the impact of regularization (Ridge/Lasso) on overfitting and coefficient values. Regularization reduced overfitting but did not outperform plain Linear Regression on this dataset.
- Tested different train-test split ratios (e.g., 80/20, 70/30) to observe effects on generalization. Results were stable across splits.
- Plotted learning curves to visualize model performance as a function of training set size, confirming sufficient data for stable results.
