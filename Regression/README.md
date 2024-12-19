## Overview
This project involves the development of a regression model to predict the target variable "total_UPDRS" using the Parkinson's disease telemonitoring dataset. The feature "motor_UPDRS" is excluded from the dataset. The approach includes preprocessing the data, performing exploratory data analysis (EDA), and building regression models, with a focus on a bidirectional LSTM recurrent network.

## Objectives
1. Load required libraries and packages.
2. Load the dataset from the specified source.
3. Conduct exploratory data analysis (EDA) as outlined in the provided document:
   - Understand the data using descriptive statistics.
   - Perform univariate visualization to understand data distributions and multivariate visualization to explore relationships between features.
   - Clean the data using appropriate methods if necessary.
   - Analyze feature correlations.
   - Experiment with combinations of features and, if required, create new features.
   - Perform feature selection to retain significant features.
   - Transform data using standardization.
4. Analyze and process the following datasets:
   - Original dataset.
   - Transformed original dataset.
   - Feature-selected dataset.
   - Transformed feature-selected dataset.
   Each dataset is split into training, validation, and test subsets.
5. Compare the performance of two models on training and validation datasets:
   - Fully connected neural network regression model.
   - Bidirectional LSTM regression model.
   Use metrics such as Root Mean Squared Error (RMSE) and R² (coefficient of determination) for evaluation.
6. Evaluate the best model on the test dataset.
7. Perform grid search to find optimal hyperparameters for the best model using training and validation datasets. Identify the best hyperparameter values.
8. Compare the performance of the best model before and after hyperparameter tuning using the test dataset.

## Methods
### Data Preprocessing
- Exclusion of "motor_UPDRS" from the dataset.
- Standardization of the data.

### Exploratory Data Analysis (EDA)
- Descriptive statistics to understand feature distributions.
- Visualization using plots to uncover patterns and correlations.
- Cleaning and feature engineering to enhance the dataset.
- Feature selection to retain the most relevant predictors.

### Models
- Fully Connected Neural Network (Baseline).
- Bidirectional LSTM Recurrent Neural Network.

### Metrics
- Root Mean Squared Error (RMSE).
- Coefficient of Determination (R²).

### Hyperparameter Optimization
- Grid search for tuning hyperparameters.
