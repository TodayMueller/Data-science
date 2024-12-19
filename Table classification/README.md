## Overview
This project focuses on building a classification model to predict the "Target" variable, which represents student dropout and academic performance. The dataset contains information collected at the time of student enrollment (academic, demographic, and socio-economic factors) and their performance at the end of the first and second semesters. The task includes preprocessing the data, conducting exploratory data analysis (EDA), and building classification models with a focus on a GRU recurrent network.

## Objectives
1. Load required libraries and packages.
2. Load the dataset from the specified source.
3. Perform exploratory data analysis (EDA) as described in the provided document:
   - Understand the data using descriptive statistics.
   - Conduct univariate visualization to explore data distributions and multivariate visualization to examine feature relationships.
   - Clean the data using appropriate methods if necessary.
   - Analyze correlations among features.
   - Experiment with feature combinations and create new features if necessary.
   - Perform feature selection to retain significant features and create a feature-selected dataset.
   - Apply min-max scaling to the data.
4. Process and analyze the following datasets:
   - Original dataset.
   - Transformed original dataset.
   - Feature-selected dataset.
   - Transformed feature-selected dataset.
   Each dataset is split into training, validation, and test subsets.
5. Compare the performance of the following models across all datasets and their transformed variants:
   - Fully connected neural network classification model.
   - GRU recurrent neural network classification model.
   Use metrics such as accuracy, balanced accuracy, and F1 score (overall and per class) for evaluation.
6. Evaluate the best model on the test dataset.
7. Perform grid search to find optimal hyperparameters for the best classification model using training and validation datasets. Identify the best hyperparameter values.
8. Compare the performance of the best model before and after hyperparameter tuning using the test dataset.

## Methods
### Data Preprocessing
- Exclusion of unnecessary features.
- Min-max scaling for feature normalization.

### Exploratory Data Analysis (EDA)
- Descriptive statistics to understand the dataset structure.
- Visualization to uncover data distributions and relationships.
- Feature engineering and selection to enhance predictive power.

### Models
- Fully Connected Neural Network (Baseline).
- GRU Recurrent Neural Network.

### Metrics
- Accuracy.
- Balanced Accuracy (for imbalanced classes).
- F1 Score (overall and per class).

### Hyperparameter Optimization
- Grid search for tuning hyperparameters.
