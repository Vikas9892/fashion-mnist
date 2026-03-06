Fashion MNIST Classification using Convolutional Neural Networks (CNN)
Overview

This project implements a Convolutional Neural Network (CNN) to classify images from the Fashion MNIST dataset. The goal is to automatically identify different categories of clothing items using deep learning techniques.

The Fashion MNIST dataset is a widely used benchmark dataset in computer vision and machine learning, consisting of grayscale images of fashion products. It serves as a more challenging alternative to the traditional MNIST handwritten digits dataset.

In this project, a CNN model is designed, trained, and evaluated to achieve high accuracy in classifying clothing images into their respective categories.

Dataset

The Fashion MNIST dataset contains:

70,000 grayscale images

Image size: 28 × 28 pixels

10 clothing categories

Classes
Label	Category
0	T-shirt / Top
1	Trouser
2	Pullover
3	Dress
4	Coat
5	Sandal
6	Shirt
7	Sneaker
8	Bag
9	Ankle Boot

Dataset split:

Training images: 60,000

Testing images: 10,000

Project Objectives

Implement a CNN-based image classification model

Train the model on the Fashion MNIST dataset

Evaluate model performance using accuracy and loss metrics

Visualize predictions and model performance

Demonstrate the effectiveness of deep learning in image recognition tasks

Model Architecture

The CNN architecture used in this project includes the following layers:

Convolutional Layers

Extract spatial features from images

Activation Function

ReLU (Rectified Linear Unit)

Pooling Layers

MaxPooling to reduce spatial dimensions

Fully Connected Layers

Combine extracted features for classification

Output Layer

Softmax activation for multi-class classification

Example architecture:

Input (28×28)
→ Conv2D
→ ReLU
→ MaxPooling
→ Conv2D
→ ReLU
→ MaxPooling
→ Flatten
→ Dense Layer
→ Softmax Output (10 classes)

Technologies Used

Python

TensorFlow / Keras

NumPy

Matplotlib

Scikit-learn

Jupyter Notebook

Installation

Clone the repository:

git clone https://github.com/your-username/fashion-mnist-cnn.git
cd fashion-mnist-cnn

Install required dependencies:

pip install -r requirements.txt
Running the Project

Run the training script:

python train.py

Or open the Jupyter notebook:

jupyter notebook fashion_mnist_cnn.ipynb
Results

The CNN model achieves strong classification performance on the Fashion MNIST dataset.

Example evaluation metrics:

Training Accuracy: ~90–95%

Test Accuracy: ~88–92%

Performance may vary depending on hyperparameters and architecture.

Sample Predictions

The trained model is able to correctly classify various clothing items such as:

Sneakers

Bags

Shirts

Dresses

Ankle Boots

Visualization of predictions helps understand the model's performance.

Project Structure
fashion-mnist-cnn/
│
├── dataset/
│
├── models/
│
├── notebooks/
│   └── fashion_mnist_cnn.ipynb
│
├── train.py
├── evaluate.py
├── requirements.txt
└── README.md
Future Improvements

Possible improvements for this project include:

Hyperparameter tuning

Data augmentation

Transfer learning with pretrained models

Model optimization for faster inference

Deployment as a web application

References

Zalando Research. Fashion-MNIST: a Novel Image Dataset for Benchmarking Machine Learning Algorithms.

TensorFlow/Keras Documentation
