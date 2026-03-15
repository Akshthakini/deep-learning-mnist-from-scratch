# deep-learning-mnist-from-scratch
Implementation of MLP, Autoencoder, and RBM from scratch using Python and NumPy on the MNIST dataset for classification, representation learning, and feature extraction.
# Deep Learning Models from Scratch using NumPy

This project demonstrates the implementation of fundamental deep learning models from scratch using Python and NumPy. The goal is to understand the internal working of neural networks without relying on high-level deep learning libraries.

## Project Overview

The project implements and analyzes three different neural network models using the MNIST handwritten digit dataset:

- Multi-Layer Perceptron (MLP) for supervised digit classification
- Autoencoder for unsupervised representation learning and reconstruction
- Restricted Boltzmann Machine (RBM) for unsupervised feature learning

The models were implemented using only basic numerical operations to gain a deeper understanding of neural network training, forward propagation, backpropagation, and representation learning.

## Dataset

The MNIST dataset consists of grayscale images of handwritten digits (0–9).

- Image size: 28 × 28 pixels  
- Input size after flattening: 784 features  
- Dataset split: Training set and Testing set  
- Pixel values normalized to the range [0,1]

## Models Implemented

### Multi-Layer Perceptron (MLP)

- Input layer: 784 neurons
- Hidden layer: ReLU activation
- Output layer: Softmax activation
- Loss function: Cross-entropy
- Optimization: Stochastic Gradient Descent

The model achieved approximately **96% test accuracy** on the MNIST dataset.

### Autoencoder

An undercomplete autoencoder was implemented to learn compressed representations of handwritten digits.

- Encoder compresses input into a lower dimensional latent space
- Decoder reconstructs the original image
- ReLU activation used in hidden layers
- Sigmoid activation used in output layer
- L1 regularization applied to enforce sparsity

The model was also used for **outlier detection using reconstruction error**.

### Restricted Boltzmann Machine (RBM)

A binary RBM was implemented for unsupervised feature learning.

- Visible layer: 784 units
- Hidden layer: 64 units
- Training algorithm: Contrastive Divergence (CD-1)

The RBM learned low-level features such as strokes and curves present in handwritten digits.

## Results

- MLP achieved strong classification accuracy.
- Autoencoder successfully reconstructed normal digits and detected outliers.
- RBM learned meaningful feature representations.

Training behavior was analyzed using:

- Loss curves
- Accuracy plots
- Reconstruction visualizations
- Feature filter visualizations

## Technologies Used

- Python
- NumPy
- Matplotlib
- MNIST Dataset

## Project Structure
