During the Day 2 tasks, I learned the difference between scaling and normalization, and explored the different approaches to preparing categorical data through encoding techniques such as one-hot and ordinal encoding.
# Burnout Breakdown – Day 2 Summary
## Data Preprocessing
- Loaded the dataset and separated columns into categorical and numerical types.
- Encoded categorical variables:
  - Used OrdinalEncoder for ordinal columns like JobRole, Department, HasMentalHealthSupport, and HasTherapyAccess.
  - Used pd.get_dummies() for nominal variables like Gender, Country, etc.
- Scaled numerical features using MinMaxScaler to bring values between 0 and 1 for better model performance.

## Feature Engineering
- Created 2 interaction features:
  - stress x workhours: Product of StressLevel × WorkHoursPerWeek
  - sleep/stress: Ratio of SleepHours / (StressLevel + 1e-5) to avoid division by zero

## Model Training
- Split the dataset into training and test sets using train_test_split().
- Trained 3 regression models:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression

- Evaluated models using:
  - Mean Squared Error (MSE)
  - R² Score

## Key Learnings:
- Encoding techniques: One-hot vs Ordinal
- Normalization using MinMaxScaler
- Interaction features improve signal strength
- Linear vs Ridge vs Lasso regression comparison
- Evaluation metrics: MSE and R²

  ## Results
  Among the three models, Ridge performed the best with the highest R² score and lowest MSE. This is might be because Ridge handles multicollinearity better by adding L2 regularization.
