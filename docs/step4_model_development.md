# Step 4: Model Development & Evaluation

In this step, we trained and evaluated a set of regression models using the features selected in Step 3.

### Models Trained:
1. **Linear Regression**
2. **Ridge Regression**
3. **Lasso Regression**
4. **Random Forest Regressor**
5. **Gradient Boosting Regressor**
6. **Stacking Regressor** (with Ridge + Lasso as base learners, and Random Forest as the final estimator)

### Evaluation Metrics:
For each model, we evaluated:
- **R² (Coefficient of Determination)**: Measures how much variance is explained by the model.
- **RMSE (Root Mean Squared Error)**: Penalizes large errors more than MAE.
- **MAE (Mean Absolute Error)**: Measures average prediction error in the same units as the target variable.

### Outcome:
- The best performing model was selected based on the highest R² score on the test set.
- All results were summarized in a comparison table and a bar chart.
