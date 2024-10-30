# denoising-autoencoder-from-scratch

## Overview

Autoencoders are a type of neural network used to learn efficient representations of data, typically for dimensionality reduction or feature learning. This project contains a PyTorch implementation of a simple one-layer autoencoder designed to encode and decode noisy handwritten digits from the MNIST dataset.

## Features

- Utilizes the MNIST dataset for training and evaluation.
- Defines both a simple and multilayer customizable autoencoder architecture.
- Includes training and evaluation scripts.

## Usage

### Model Structure

The autoencoder structure is simple, consisting of:
- **Encoder**: A single linear layer that compresses the 784-dimensional input down to a latent space.
- **Decoder**: A single linear layer that reconstructs the input from the latent space back to the original dimension.

### Evaluation

The script includes validation and test loaders to evaluate the model performance after training. You can customize the batch size and training parameters as desired.

### Data

The MNIST dataset is downloaded automatically from Keras, and it is split into training/test sets. The data is reshaped into 28x28 images for easy manipulation.

## Dependencies

- Python >= 3.6
- PyTorch
- torchvision
- numpy
- tqdm
- keras

## Results

The trained autoencoder can effectively compress and reconstruct images of handwritten digits (even when noisy) from the MNIST dataset, demonstrating dimensionality reduction capabilities.
