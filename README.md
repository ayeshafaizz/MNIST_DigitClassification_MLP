MNIST Digit Classification using Multi-Layer Perceptron (MLP)

## Project Overview

This project focuses on building and training a Multi-Layer Perceptron (MLP) using TensorFlow/Keras for handwritten digit classification on the MNIST dataset. The goal was to understand the complete deep learning workflow, including data preprocessing, neural network design, regularization techniques, callback usage, and performance evaluation.

The model was enhanced using Batch Normalization, Dropout, Early Stopping, Model Checkpointing, and TensorBoard logging to improve training stability and generalization performance.

---

## Dataset

**MNIST Handwritten Digits Dataset**

* 70,000 grayscale images
* Image size: 28 × 28 pixels
* 10 digit classes (0–9)
* Training samples: 60,000
* Testing samples: 10,000

---

## Objectives

* Load and preprocess image data
* Build a deep neural network using Keras Sequential API
* Apply Batch Normalization and Dropout
* Prevent overfitting using EarlyStopping
* Save the best model using ModelCheckpoint
* Monitor training using TensorBoard
* Achieve test accuracy above 97%

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* TensorFlow
* Keras
* TensorBoard

---

## Project Workflow

### 1. Data Loading

* Loaded MNIST dataset from Keras datasets.

### 2. Data Preprocessing

* Flattened 28×28 images into 784-dimensional vectors.
* Normalized pixel values to the range [0,1].

### 3. Model Architecture

Input Layer:

* 784 features

Hidden Layers:

* Dense(512, ReLU)

* BatchNormalization

* Dropout(0.3)

* Dense(256, ReLU)

* BatchNormalization

* Dropout(0.3)

* Dense(128, ReLU)

* BatchNormalization

* Dropout(0.3)

Output Layer:

* Dense(10, Softmax)

### 4. Training Configuration

* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy
* Metric: Accuracy
* Batch Size: 128
* Validation Split: 20%

### 5. Callbacks

* EarlyStopping
* ModelCheckpoint
* TensorBoard

### 6. Evaluation

* Training Accuracy Analysis
* Validation Accuracy Analysis
* Test Set Evaluation
* Prediction Visualization

---

## Results

| Metric              | Value  |
| ------------------- | ------ |
| Training Accuracy   | 98.4%  |
| Validation Accuracy | 98.18% |
| Test Accuracy       | 98.10% |
| Test Loss           | 0.0622 |

---

## Key Learnings

* Implemented a complete neural network using TensorFlow/Keras.
* Learned the role of Batch Normalization in stabilizing training.
* Understood how Dropout reduces overfitting.
* Used EarlyStopping to avoid unnecessary training.
* Saved the best-performing model with ModelCheckpoint.
* Monitored model performance through TensorBoard.
* Achieved high accuracy on a real-world image classification task.

---

## Files Included

* `MNIST_MLP_Keras.ipynb`
* `best_mnist_model.keras`
* `mnist_mlp_final.keras`
* `README.md`

---

## Conclusion

The Multi-Layer Perceptron successfully classified handwritten digits with a test accuracy of 98.10%, exceeding the project target of 97%. This project provided practical experience with TensorFlow/Keras and introduced essential deep learning concepts such as neural network architecture design, regularization, callback usage, and model evaluation.

