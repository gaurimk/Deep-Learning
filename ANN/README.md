# 🧠 Artificial Neural Network (ANN)

This project implements a basic Artificial Neural Network (ANN) for supervised learning tasks.  
An ANN is a network of interconnected neurons organized in layers that can learn complex, non-linear relationships from data.

---

## 🔍 Overview

An ANN typically consists of:

- **Input layer** – receives the input features  
- **Hidden layer(s)** – performs transformations and learns patterns  
- **Output layer** – produces final predictions  

The network is trained using **backpropagation** and **gradient descent**, where weights are updated to minimize a chosen loss function.

---

## 🛠️ Features

✔ Implementation of a feed-forward ANN  
✔ Support for multiple hidden layers  
✔ Activation functions such as ReLU / Sigmoid  
✔ Training using backpropagation and gradient-based optimization  
✔ Evaluation using accuracy and loss  
✔ Easy to adapt for classification or regression tasks  

---

## 🧩 How It Works

A single neuron in the network computes:

$$
z = w \cdot x + b
$$

where:

- $w$ – weight vector  
- $x$ – input vector  
- $b$ – bias term  

The neuron then applies an **activation function** $f$:

$$
a = f(z)
$$

Example activations:

- **Sigmoid** (for binary classification):

$$
\sigma(z) = \frac{1}{1 + e^{-z}}
$$

- **ReLU**:

$$
\text{ReLU}(z) = \max(0, z)
$$

---

### 🔁 Training with Backpropagation

1. **Forward Pass**  
   Inputs are propagated layer by layer to compute the output $\hat{y}$.

2. **Loss Computation**  
   A loss function $L(y, \hat{y})$ measures the error between true label $y$ and prediction $\hat{y}$.

   Example (binary cross-entropy):

   $$
   L(y, \hat{y}) = - \big[ y \log(\hat{y}) + (1 - y)\log(1 - \hat{y}) \big]
   $$

3. **Backward Pass**  
   Gradients of the loss with respect to each weight are computed using the chain rule.

4. **Weight Update**  
   Weights are updated using gradient descent:

   $$
   w_{new} = w_{old} - \eta \frac{\partial L}{\partial w}
   $$

   where $\eta$ is the learning rate.

---

## 📁 Project Structure

```text
Project/
│
├── ann.py or notebook.ipynb      # ANN implementation and training code
├── data/                         # Optional dataset folder
└── README.md                     # Project documentation
