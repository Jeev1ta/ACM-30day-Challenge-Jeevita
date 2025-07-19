During the Day 4 task, I learned how decision trees work, explored the Random Forest algorithm including its advantages and how it aggregates multiple trees, and implemented k-NN for classification. I also studied the core algorithm behind Random Forest and understood how k-NN makes predictions based on similarity.
## Work Done:
- Initial Preprocessing
  - Loaded and cleaned dataset
  - Encoded categorical variables using get_dummies()
  - Scaled numeric features using StandardScaler
- Model Training (Full Features)
  - Trained:
    - Decision Tree Classifier
    - Random Forest Classifier
    - k-Nearest Neighbors Classifier
  - Evaluated models using Accuracy Score and Confusion Matrix
- Feature Importance + Selection
  - Used Random Forest Feature Importance to rank features
  - Selected top 3 most important features based on importance scores
  - Optionally verified with Mutual Information or Correlation Matrix
- Reduced Feature Model Challenge
  - Re-trained all 3 models using only the top 3 features
  - Compared performance of full-feature vs reduced-feature models
 
## Before vs After: Model Comparison
| Model         | Accuracy (All Features) | Accuracy (Top 3 Features) |
| ------------- | ----------------------- | ------------------------- |
| Decision Tree |         0.53            |           0.54            |
| Random Forest |         0.67            |           0.63            |
| k-NN          |         0.60            |           0.58            |

## Key Learnings:
- Tree-based models can give direct insights into feature importance.
- Using feature selection (like Random Forest importance) helps simplify models and reduce overfitting.
- Performance often drops slightly with fewer features, but sometimes not significantly—showing those features capture most signal.
- Tradeoff between simplicity vs performance is crucial in real-world ML.
