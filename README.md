
# Car Price Prediction using Linear and Regularized Regression Techniques

## Overview
The goal of this project is to build a predictive model to estimate car prices based on various attributes using the CarPrice_Assignment dataset. The dataset contains 205 instances and 26 features related to car specifications.

## Contents

### A. Data Summary
- Loaded the dataset and examined its structure (205 rows, 26 columns)
- Identified continuous and categorical features
- Provided statistical summaries for numerical attributes

### B. Visualization & Statistical Analysis
- Plotted histograms to analyze distributions of all features
- Identified traits such as skewness, clusters, and outliers

### C. Correlation & Attribute Relationships
- Computed Pearson Correlation Coefficients
- Created scatter plots and heatmaps
- Observed strong positive correlation (e.g., horsepower vs. price)

### D. Train-Test Split
- Used `train_test_split` to divide the data (80% training, 20% testing)
- Verified representativeness of test set by comparing summary statistics

### E. Model Building & Evaluation
- Built and evaluated a Linear Regression model using 4-fold cross-validation
- Implemented Ridge, Lasso, and ElasticNet regressions with various alpha values
- Compared R² scores to assess performance

### F. Stochastic Gradient Descent (SGD)
- Evaluated impact of batch size and learning rate on loss
- Tracked mean squared error for training and validation sets
- Visualized convergence over iterations

### G. Polynomial Regression
- Tested polynomial regression with degrees 1 to 4
- Degree 1 yielded the best validation performance
- Detected overfitting with higher degrees via increased validation loss

### H. Final Model & Prediction
- Selected Linear Regression (degree 1) as the final model
- Achieved R² score of ~0.8656 on test data
- Discussed future improvements such as feature scaling, outlier handling, and advanced models

## Technologies Used
- Python 3.x
- NumPy, Pandas, Matplotlib, Seaborn
- Scikit-learn (Linear Models, Cross-Validation, Pipelines)

## Conclusion
The best-performing model is Linear Regression with Ridge Regularization (α = 0.1), yielding an R² score of ~0.8656. Polynomial models beyond degree 1 showed overfitting. Improvements can be made with more advanced preprocessing and modeling strategies.
