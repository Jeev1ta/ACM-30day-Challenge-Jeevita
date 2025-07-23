# Breakdown of cycle - 2, phase - 1:

## Data Preparation
- Loaded the Breast Cancer dataset from Kaggle.
- Dropped irrelevant column.
- Encoded the target.
- Verified data types and null values.
- Split into features and labels.
  
## Model Training
- Trained the following ensemble models:
  - RandomForestClassifier (Bagging)
  - AdaBoostClassifier (Boosting)
  - XGBoostClassifier (Boosting)
- Used an 80/20 train-test split.

## Evaluation
- Measured and compared model accuracy using accuracy_score.
- Visualized model performance with a bar chart showing all three accuracies.
