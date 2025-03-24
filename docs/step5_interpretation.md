# Step 5: Model Interpretation

This step focused on interpreting the best-performing model identified in Step 4.

### What We Did:
- If the best model was **tree-based** (e.g., Random Forest), we extracted and ranked its `feature_importances_`.
- If it was **linear** (e.g., Lasso), we extracted the coefficient weights from `model.coef_`.

### Visualization:
- We plotted the **top 10 features** influencing the predictions.
- A horizontal bar chart was used to visualize the magnitude of influence for interpretability.

### Purpose:
- Understanding which features have the greatest positive or negative impact on the predicted final grade.
- Supports actionable insights and possible intervention strategies in education.
