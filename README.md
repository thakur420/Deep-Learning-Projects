# 🧠 Deep Learning Projects

This repository contains deep learning projects implemented **from scratch** using **Python and NumPy**, as well as using the **TensorFlow Keras** framework for comparison and experimentation.

---

## 📘 Overview

This project demonstrates how deep learning models can be built both:
1. **From scratch** — implementing every component manually (forward pass, backpropagation, gradient descent).
2. **Using TensorFlow Keras** — leveraging a high-level API for efficient model training and experimentation.

---

## 📁 Project Structure

| Notebook | Description |
|-----------|--------------|
| `Neural_Net_from_Scratch.ipynb` | Implements a **fully connected neural network (MLP)** from scratch using only NumPy. |
| `Neural_Net_Using_Framework.ipynb` | Implements **MLP and CNN** models using the **TensorFlow Keras** framework. |

---

## ✨ Features

- Implementation of **forward and backward propagation**
- Supports **multiple (deep) layers**
- Activation functions: **Sigmoid**, **ReLU**, and **Tanh**
- Implements **Binary Cross-Entropy loss**
- Training with **gradient descent**
- Trained and Evaluated on **CIFAR-10(Cats vs Dogs subset)**

---

## 🧠 Model Performance Summary

Here's a summary of the performance on the test set for each model:

| 🧩 **Model** | ⚙️ **Train Accuracy** | 🧪 **Test Accuracy** | 📊 **Remarks** |
|:-------------|:--------------------:|:--------------------:|:----------------|
| **MLP Model (Implemented from Scratch)** | 85% | 60% | ⚠️ Overfitting — No convolution or augmentation used |
| MLP Model | 98% | 61% | ⚠️ Overfitting |
| Basic CNN Model | 93% | 73% | ✅ Stable baseline |
| CNN with BN and Dropout (LeNet-5 style) | 80% | 75% | 👍 Better generalization |
| CNN with Data Augmentation (LeNet-5 style) | 80% | 76% | 📈 Slight improvement |
| Larger CNN with Data Augmentation | 99% | 83% | ⚠️ Overfitting sign |
| **Transfer Learning with EfficientNetB0** | **92%** | **91% 🏆** | 🌟 Best performance |
---
> 🏁 **Conclusion:** The EfficientNetB0 model achieved the highest test accuracy, showing the benefit of transfer learning.

## ⚙️ Getting Started

### 🧩 Prerequisites

Make sure you have the following installed:
- Python 3.x  
- NumPy  
- Jupyter Notebook  
- TensorFlow (for framework-based models)

### 📦 Installation

Clone this repository:
```bash
git clone https://github.com/thakur420/Deep-Learning-Projects.git
cd deep-learning-projects
