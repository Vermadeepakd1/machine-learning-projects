# 📌 Project: Titanic Survival Prediction

## Problem

Predict which passengers survived the Titanic disaster using classification models.

## Dataset

- Source: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)
- Description: Classic binary classification dataset with features such as Pclass, Sex, Age, SibSp, Parch, Fare, Embarked, and the target variable Survived. Includes both train and test sets.

## Steps Performed

- Exploratory Data Analysis (EDA)
- Data cleaning (handling missing values, removing unnecessary columns)
- Feature engineering (FamilySize, IsAlone)
- Encoding categorical variables
- Feature scaling
- Model training (Logistic Regression)
- Evaluation (accuracy, confusion matrix, classification report)
- Submission file creation for Kaggle

## Model Used

- Logistic Regression

## Results

- Accuracy (Logistic Regression): ~80% (based on typical splits)
- Most important features: Sex, Pclass, Fare, FamilySize
- Confusion matrix and classification report used for detailed evaluation

## Key Learnings

- Sex and Pclass are the strongest predictors of survival.
- Feature engineering (FamilySize, IsAlone) can improve model performance.
- Handling missing values and outliers (e.g., Age, Fare) is crucial for robust predictions.
- Logistic Regression provides a strong baseline for binary classification on this dataset.

---

### 🧪 Experiments

- Compared model performance with and without feature scaling (StandardScaler)
- Analyzed the impact of feature engineering (FamilySize, IsAlone)
- Tested different train-test split ratios (e.g., 70/30, 80/20)
- Evaluated model using accuracy, confusion matrix, and classification report

This project demonstrates a complete applied machine learning workflow for a classic classification problem.
