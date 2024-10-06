# MNIST Digit Classifier with TensorFlow

## Description

This project implements a neural network to classify handwritten digits from the MNIST dataset using TensorFlow and Keras. 
The model is trained to recognize digits (0-9) from 28x28 grayscale images, then evaluated for accuracy on test data. 
Finally, the model predicts digits from unseen test samples.

## Requirements

- Python 3.x
- TensorFlow 2.x
- Matplotlib (for visualization)

## How It Works

- **Data Loading**: The MNIST dataset, which contains 60,000 training images and 10,000 test images, is loaded using TensorFlow.
- **Preprocessing**: The pixel values are normalized to be between 0 and 1 for faster convergence during training.
- **Model Architecture**: A simple neural network is built with:
  - **Input layer**: Flatten the 28x28 images into a 1D vector.
  - **Hidden layer**: 128 neurons with ReLU activation.
  - **Output layer**: 10 neurons with softmax activation for classification into one of 10 digit classes.
- **Training**: The model is trained using the Adam optimizer and sparse categorical crossentropy loss.
- **Evaluation**: The model is evaluated on test data, and its accuracy is printed.
- **Prediction**: The model predicts the first 5 test images, and the results are displayed with their respective predicted digits.

## Running the Code

1. Clone or download the repository.
2. Open the project in your IDE or use Google Colab.
3. Run the script to train the model and visualize predictions.

## Output

The model will output the accuracy of the test set and display the first 5 test images with their predicted labels.
