# 🧠 Perceptron Algorithm

The Perceptron is the simplest type of Artificial Neural Network — a single-layer binary classifier.  
This project demonstrates how the Perceptron learns decision boundaries through iterative weight updates.

---

## 🔍 Overview

The Perceptron algorithm is used for supervised learning of linearly separable classification tasks.  
It adjusts model weights based on prediction errors until the classifier converges.

---

## 🛠️ Features

✔ Implementation of Perceptron from scratch  
✔ Binary classification task  
✔ Weight update using Perceptron Learning Rule  
✔ Visualization of decision boundary (if using 2D data)  
✔ Easy to edit and extend for custom datasets  

---

## 🧩 How It Works

The Perceptron updates weights using:

$$
w_{new} = w_{old} + \eta (y - \hat{y})x
$$

Where:

| Symbol | Meaning |
|--------|---------|
| $w$ | Weight vector |
| $\eta$ | Learning rate |
| $y$ | True label |
| $\hat{y}$ | Predicted label |
| $x$ | Input vector |

Activation Function:

$$
\hat{y} =
\begin{cases}
1 & \text{if } (w \cdot x + b) \ge 0 \\
0 & \text{otherwise}
\end{cases}
$$

---

## 📁 Project Structure

```text
Project/
│
├── perceptron.py or notebook.ipynb
├── data/ (optional dataset folder)
└── README.md
