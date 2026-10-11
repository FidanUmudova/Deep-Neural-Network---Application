# Deep Learning Specialization: Course 1 (Week 4 - Neural Network Model Exercises)

This repository contains the solutions to key practical programming exercises from Week 4 of Course 1 ("Neural Networks and Deep Learning") of the Deep Learning Specialization by DeepLearning.AI, taught by Andrew Ng.

---

## 🚀 Implemented Models (Exercises)

This project features two main neural network architectures built completely from scratch using NumPy:

### 1. Two-Layer Neural Network (`two_layer_model`)
* **Architecture:** `LINEAR -> RELU -> LINEAR -> SIGMOID`
* **Description:** This function implements a complete optimization loop for binary image classification (e.g., cat vs. non-cat). It handles parameter initialization, forward propagation, cost computation, backpropagation, and gradient descent updates.

### 2. L-Layer Deep Neural Network (`L_layer_model`)
* **Architecture:** `[LINEAR -> RELU] × (L-1) -> LINEAR -> SIGMOID`
* **Description:** A universal model of arbitrary depth ($L$ layers). It allows dynamic network configuration via the `layers_dims` list, integrating all modular deep learning helper functions (`initialize_parameters_deep`, `L_model_forward`, `compute_cost`, `L_model_backward`, `update_parameters`).

---

## 🛠️ Core Functions

| Function | Description |
| :--- | :--- |
| `two_layer_model(...)` | Trains a 2-layer neural network through a gradient descent optimization loop. |
| `L_layer_model(...)` | Trains a deep $L$-layer neural network with customizable depth. |
| `initialize_parameters_deep(layers_dims)` | Dynamically initializes weights ($W$) and biases ($b$) for any network depth. |
| `L_model_forward(X, parameters)` | Performs a complete forward propagation pass across all $L$ layers. |
| `L_model_backward(AL, Y, caches)` | Performs backpropagation through all layers in reverse order. |

---
