# MNIST Digit Classification Using a Neural Network

## About the Project

This project is part of my Artificial Intelligence internship with Naviotech.

The goal of the project is to build a neural network that can recognize handwritten digits from 0 to 9 using the MNIST dataset.

I worked through the complete machine-learning workflow, starting with preparing the image data and ending with testing the trained model on a separate handwritten digit image.

## What I Built

The project includes:

- Loading and exploring the MNIST dataset
- Preparing and normalizing the image data
- Building a neural network using TensorFlow/Keras
- Training the model on handwritten digit images
- Evaluating the model on unseen test data
- Generating predictions for test images
- Using a confusion matrix to understand classification performance
- Testing the trained model on an external handwritten digit image

## Dataset

The project uses the MNIST handwritten-digit dataset.

It contains:

- 60,000 training images
- 10,000 test images
- Image size: 28 × 28 pixels
- Grayscale images
- 10 classes, representing digits 0 through 9

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- OpenCV
- Google Colab

## Data Preparation

The image data is normalized so pixel values are represented from 0 to 1 instead of 0 to 255.

For the external handwritten image, the image is:

1. Loaded using OpenCV
2. Converted to grayscale
3. Resized to 28 × 28 pixels
4. Normalized
5. Reshaped for the neural network

## Neural Network

The model is a simple feed-forward neural network:

```text
Input Image (28 × 28)
        ↓
Flatten
        ↓
Dense Layer — 50 neurons — ReLU
        ↓
Dense Layer — 50 neurons — ReLU
        ↓
Output Layer — 10 neurons — Softmax
```

The ten output neurons represent digits 0 through 9.

## Model Configuration

- Optimizer: Adam
- Loss function: Sparse Categorical Crossentropy
- Metric: Accuracy
- Training: 10 epochs

## Results

| Metric | Result |
|---|---:|
| Training Accuracy | Approximately 98.99% |
| Test Accuracy | Approximately 97.09% |
| Test Loss | Approximately 0.1182 |

The model performed well on the unseen MNIST test data.

## Single-Image Prediction

As an additional test, I used a separate handwritten image containing the digit 3.

The trained model correctly recognized it as:

**Predicted Digit: 3**

This demonstrates that the trained model can also classify a separately supplied handwritten image after preprocessing.

## Project Structure

```text
MNIST-Digit-Classification-Naviotech/
│
├── MNIST_Digit_Classification_Naviotech.ipynb
├── MNIST_Digit_Classification_Naviotech_Polished.pptx
├── 3-digit.PNG
└── README.md
```

## How to Run the Project

The notebook was developed in Google Colab.

1. Open Google Colab.
2. Upload `MNIST_Digit_Classification_Naviotech.ipynb`.
3. Run the notebook cells from the beginning in order.
4. Make sure the required libraries are available.
5. For the external-image prediction section, provide the path to the handwritten digit image.
6. The model will process the image and display the predicted digit.

## Conclusion

This project helped me understand the complete workflow of a basic image-classification problem using a neural network.

The model achieved approximately 97.09% accuracy on the MNIST test dataset and successfully recognized the separate handwritten digit 3 as 3.

The project demonstrates the process from data preparation and neural-network design to model training, evaluation, and real-image prediction.

## Author

**Ankit Dagar**

Artificial Intelligence Internship Project  
**Naviotech**
