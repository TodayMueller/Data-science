## Overview
This project aims to classify images of flowers into five distinct classes using two neural network approaches:
1. Convolutional Neural Network (CNN) with multiple Conv2D and MaxPooling layers followed by a two-layer fully connected neural network.
2. Fully Connected Neural Network (FCNN) with pretraining using an unsupervised learning technique such as autoencoder or restricted Boltzmann machine (RBM).

The project involves training, validation, and testing phases, as well as performance evaluation through accuracy and loss metrics. Data augmentation, batch training, regularization, and dropout techniques are applied to improve generalization and reduce overfitting.

## Objectives
1. Build and train a **Convolutional Neural Network (CNN)** for flower image classification:
   - Use multiple pairs of Conv2D and MaxPooling layers.
   - Final layers consist of a two-layer fully connected neural network for classification into 5 classes.
   - Validate the model during training.
   - Evaluate training and validation accuracy and loss.
   - Plot accuracy and loss graphs.
   - Test the trained CNN on a separate test dataset.

2. Build and train a **Fully Connected Neural Network (FCNN)** with pretraining:
   - Pretrain the network using an autoencoder or RBM.
   - Train the FCNN for flower image classification.
   - Validate the model during training.
   - Evaluate training and validation accuracy and loss.
   - Plot accuracy and loss graphs.
   - Test the trained FCNN on a separate test dataset.

3. Compare the performance of the CNN and FCNN models:
   - Compare training and validation accuracy.
   - Compare training and validation loss.

## Methods
### Data Augmentation
- Use image generators to expand the dataset through transformations such as rotation, zoom, and flipping.

### Training Techniques
- Batch training to handle large datasets.
- Regularization techniques to prevent overfitting.
- Dropout layers for improved generalization.

### Metrics
- **Accuracy**: Evaluated on training, validation, and test datasets.
- **Loss**: Monitored during training and validation phases.
