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
- Decision Tree Classifier (with and without max_depth pruning)

## Results

### Model Results Table (Portfolio-Ready Clarity)

| Model                      | Train Acc | Test Acc |
| -------------------------- | --------- | -------- |
| Logistic Regression        | 0.81      | 0.77     |
| Decision Tree (depth=None) | 0.83      | 0.77     |
| Decision Tree (depth=3)    | 0.81      | 0.82     |

- Most important features: Sex, Pclass, Fare, FamilySize
- Confusion matrix and classification report used for detailed evaluation

## Key Learnings

- Sex is the most important feature.
- Pclass is more important than Age.
- Some engineered features (like IsAlone) have low impact.
- Embarked has minimal effect compared to other features.

**Takeaway:**

Decision Trees can easily overfit small datasets like Titanic, but pruning helps control variance. Compared to Logistic Regression, trees capture non-linear patterns but require careful tuning.

## Decision Tree Modeling

- Implemented Decision Tree Classifier to compare with Logistic Regression.
- Evaluated both unpruned (default) and pruned (max_depth=3) trees to observe overfitting and generalization.
- Used feature importances to interpret which variables most influenced survival predictions.
- Demonstrated that pruning (max_depth=3) improved test accuracy and reduced overfitting.
- Visualized the tree structure for interpretability.

**Key Insights:**

- Decision Trees can model non-linear relationships and interactions between features.
- Pruning is essential to prevent overfitting, especially on small datasets.
- Feature importance from trees provides valuable interpretability for business and domain understanding.

---

### 🧪 Experiments

- Compared model performance with and without feature scaling (StandardScaler)
- Analyzed the impact of feature engineering (FamilySize, IsAlone)
- Tested different train-test split ratios (e.g., 70/30, 80/20)
- Evaluated model using accuracy, confusion matrix, and classification report

This project demonstrates a complete applied machine learning workflow for a classic classification problem.
