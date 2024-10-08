# Digit-Recognizer
[![Kaggle](https://img.shields.io/badge/kaggle-competitions-blue)](https://kaggle.com) 
[![PyTorch](https://img.shields.io/badge/PyTorch-latest-red?logo=pytorch)](https://pytorch.org)
This project implements a Convolutional Neural Network (CNN) to classify handwritten digits (0-9) using the MNIST dataset. The model is built using PyTorch and achieves high accuracy on the MNIST test set.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [How to Run the Project](#how-to-run-the-project)
- [Results](#results)
- [Project Structure](#project-structure)
- [References](#references)

---

## Project Overview

The goal of this project is to develop a deep learning model capable of recognizing handwritten digits with high accuracy. The project includes data preparation, model training, evaluation, and prediction.

---

## Dataset

- **Source:** [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)
- **Training Samples:** 60,000 images (28x28 grayscale)
- **Test Samples:** 10,000 images (28x28 grayscale)
- **Classes:** Digits 0 to 9

---

## Model Architecture

The model is based on a simple CNN architecture inspired by **LeNet-5**:
- 2 Convolutional Layers
- 2 Max Pooling Layers
- 3 Fully Connected Layers
- ReLU Activations and Softmax Output

---

## Training

- **Loss Function:** CrossEntropyLoss
- **Optimizer:** Adam with a learning rate of 0.001
- **Epochs:** 5

---
## Results

The Convolutional Neural Network (CNN) trained on the MNIST dataset achieves the following results:

- **Training Accuracy:** ~99.9%
- **Validation Accuracy:** ~98.7%

---

## References

Below are the references for the tools, libraries, and datasets used in this project:

- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html) – Official documentation for PyTorch, the deep learning framework used in this project.
- [Torchvision MNIST Dataset](https://pytorch.org/vision/stable/datasets.html#mnist) – The MNIST dataset used in the project, provided by PyTorch's `torchvision` package.
- [LeNet-5 Paper](http://yann.lecun.com/exdb/lenet/) – The original paper describing the LeNet-5 architecture, used as inspiration for the CNN model in this project.
- [Kaggle: Digit Recognizer](https://www.kaggle.com/c/digit-recognizer/data) – Kaggle's digit recognizer competition using the MNIST dataset.


## How to Run the Project

### 1. **Install Dependencies**
Ensure you have the required Python packages:
```bash
pip install torch torchvision matplotlib seaborn
