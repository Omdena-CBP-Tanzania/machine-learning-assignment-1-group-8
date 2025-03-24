# Step 3: Feature Engineering & Selection

This step involves identifying the most predictive features for use in the regression model. The process includes the following sub-steps:

### 1. Top Correlated Features
- We compute the absolute Pearson correlation of all features with the target variable `final_grade`.
- The top 15 features with the highest absolute correlation are selected for further consideration.

### 2. Multicollinearity Check
- We calculate the correlation matrix of the top features.
- If any two features have a correlation greater than 0.85, one of them is dropped to avoid redundancy and multicollinearity.

### 3. Feature Selection with RFE
- Recursive Feature Elimination (RFE) is applied using a Linear Regression model.
- It iteratively removes the least significant features until only the top 10 are retained.

### 4. Feature Selection with Lasso
- Lasso regression is used for embedded feature selection by penalizing less important coefficients.
- Features with zero coefficients are dropped.

### 5. Final Features
- The final feature set is derived by taking the **intersection of RFE and Lasso** selected features.
- This ensures that the selected variables are both statistically significant and robust to regularization.

The resulting set of features is then used to train and evaluate our models in the next step.
