## Overview
This project focuses on sentiment analysis of movie reviews from the IMDB dataset using two neural network architectures:
1. A bidirectional Long Short-Term Memory (BiLSTM) recurrent neural network.
2. A fully connected neural network enhanced with unsupervised pretraining using an autoencoder.

The goal is to classify reviews into two categories: **positive** and **negative**, based on the textual content of the reviews.

---

## Dataset Description
The dataset contains 50,000 movie reviews:
- **Training set**: 25,000 reviews (50% positive, 50% negative).
- **Validation and test sets**: Split from the remaining 25,000 reviews, maintaining the 50/50 class balance.

Each review is labeled as either positive or negative, making this a binary classification problem.

---

## Project Objectives
1. **Preprocessing**:
   - Tokenize and pad text sequences to ensure uniform input size.
   - Create training, validation, and test sets.

2. **Model Development**:
   - **Model 1**: BiLSTM recurrent neural network for capturing sequential dependencies in text.
   - **Model 2**: Fully connected neural network with unsupervised pretraining using an autoencoder for feature extraction.

3. **Training**:
   - Train each model on the training set using cross-entropy loss and Adam optimizer.
   - Regularization techniques, such as dropout and early stopping, to prevent overfitting.

4. **Evaluation**:
   - Evaluate both models on the validation and test sets using the following metrics:
     - Accuracy
     - F1-score (overall and per class)
   - Compare performance metrics and loss curves across models.

5. **Visualization**:
   - Plot accuracy and loss curves for both training and validation.
   - Compare evaluation metrics (e.g., accuracy, F1-score) for the two models.

---

## Implementation Steps
### Data Preprocessing
- Import IMDB dataset from Keras datasets module.
- Preprocess text data: tokenization, padding, and splitting into training, validation, and test sets.

### Model Architectures
#### Model 1: BiLSTM Recurrent Neural Network
- Input layer: Embedding layer to convert tokens to dense vectors.
- Hidden layers: Bidirectional LSTM layers for sequential dependency modeling.
- Output layer: Dense layer with sigmoid activation for binary classification.

#### Model 2: Fully Connected Neural Network with Autoencoder Pretraining
- **Autoencoder Pretraining**:
  - Train an autoencoder to extract features from the input data.
  - Use the encoder part of the autoencoder as the feature extractor.
- **Classification Network**:
  - Input: Features from the autoencoder.
  - Hidden layers: Dense layers with ReLU activation.
  - Output layer: Dense layer with sigmoid activation.

### Training and Hyperparameter Tuning
- Use grid search for hyperparameter optimization.
- Tune parameters like learning rate, batch size, and dropout rate.

### Evaluation
- Compute accuracy and F1-score on validation and test sets.
- Compare performance before and after hyperparameter tuning.
