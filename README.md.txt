# MNIST Digit Classification using Neural Networks

## Project Overview

This project implements a simple Artificial Neural Network to classify handwritten digits from 0 to 9 using the MNIST dataset.

The project demonstrates the complete workflow of an image-classification system, including dataset loading, data preprocessing, neural-network development, model training, evaluation, prediction, and single-image digit recognition.

## Objective

The objective of this project is to build and train a neural network capable of recognizing handwritten digits from 0 to 9 using the MNIST dataset.

## Dataset

The MNIST dataset contains:

- 60,000 training images
- 10,000 test images
- Image size: 28 × 28 pixels
- Grayscale images
- Digit classes: 0 to 9

Each image represents a handwritten digit.

## Technologies Used

- Python
- Google Colab
- TensorFlow / Keras
- NumPy
- Matplotlib
- OpenCV

## Project Workflow

The project follows these major steps:

1. Import required libraries
2. Load the MNIST dataset
3. Understand the dataset structure
4. Visualize sample images
5. Normalize image pixel values
6. Build the neural-network model
7. Compile the model
8. Train the neural network
9. Evaluate the model
10. Generate predictions
11. Analyze predictions using a confusion matrix
12. Predict a single handwritten digit image

## Data Preprocessing

The MNIST images contain pixel values ranging from 0 to 255.

To make the training process more efficient, the pixel values are normalized to a range between 0 and 1.

The normalization is performed using:

```python
x_train = x_train / 255.0
x_test = x_test / 255.0