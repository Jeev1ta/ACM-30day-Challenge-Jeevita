# Day 3 - Breakdown
## Objective:
- Build classifiers to predict burnout (0 = No, 1 = Yes) and evaluate them using accuracy, confusion matrix, and ROC-AUC.

## Work Done:
- Converted Target Variable
  - Mapped BurnoutRisk from "Yes"/"No" to binary (1/0).

- Encoded Categorical Data
  - Used pd.get_dummies() to convert categorical columns into numerical format.

- Scaled Numerical Features
  - Applied StandardScaler to normalize numerical columns before model training.

- Trained Models
  - Logistic Regression without LDA: Trained on the original scaled and encoded features.
  - LDA + Logistic Regression: Reduced dimensions using Linear Discriminant Analysis (LDA), then trained Logistic Regression on the transformed data.

- Evaluated Models
  - Accuracy Score: Checked how often the model predicted correctly.
  - Confusion Matrix: Evaluated True/False Positives and Negatives.
  - ROC Curve + AUC: Plotted ROC curve and calculated AUC score to measure classifier performance.

## Visualizations:
- ROC Curve for Logistic Regression
- ROC Curve for LDA + Logistic Regression

## Key Learnings:
- Difference between dimensionality reduction (LDA) and classification.
- How LDA can be used before Logistic Regression to simplify feature space.
- Importance of evaluation metrics beyond accuracy — especially ROC-AUC when dealing with class imbalance.
- Practice with binary classification workflows in scikit-learn.
