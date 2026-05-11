# TensorFlow Playground – Deep Learning Fundamentals

This project focuses on understanding the fundamentals of Deep Learning using TensorFlow Playground and TensorFlow/Keras.

The goal of this exercise is to visually explore how neural networks work, how layers and neurons interact, and how activation functions affect model performance.

---

# Project Objectives

- Understand the basic structure of Neural Networks
- Explore hidden layers and neuron behavior
- Learn the importance of activation functions
- Compare classification and regression tasks
- Analyze XOR and Spiral datasets
- Build simple neural network architectures with TensorFlow/Keras

---

# Technologies Used

- Python
- TensorFlow
- Keras
- Jupyter Notebook
- TensorFlow Playground

---

# Topics Covered

## 1. Deep Learning Classification

- Binary classification
- Decision boundaries
- Hidden layers
- Activation functions
- ReLU vs Linear
- Feature engineering concepts

---

## 2. Neural Network Architecture

Created neural network models with:

- Input layers
- Multiple hidden layers
- ReLU activation
- Sigmoid output layer

Example architecture:

```python
model = Sequential()

model.add(Input(shape=(2,)))

model.add(layers.Dense(5, activation="relu"))
model.add(layers.Dense(4, activation="relu"))
model.add(layers.Dense(3, activation="relu"))

model.add(layers.Dense(1, activation="sigmoid"))
```

---

## 3. Parameter Calculation

Learned how to manually calculate trainable parameters in neural networks.

Formula:

```text
(inputs × neurons) + bias
```

---

## 4. XOR Dataset

Implemented a neural network for solving the XOR problem.

Why important?

- XOR is not linearly separable
- Requires hidden layers
- Demonstrates the power of non-linear activation functions

Architecture:

```python
xor_model = Sequential()

xor_model.add(Input(shape=(2,)))

xor_model.add(layers.Dense(4, activation="relu"))
xor_model.add(layers.Dense(4, activation="relu"))

xor_model.add(layers.Dense(1, activation="sigmoid"))
```

---

## 5. Spiral Dataset

Designed a deeper neural network for the Spiral dataset.

Why deeper?

- Spiral data is highly non-linear
- Requires more neurons and layers
- Demonstrates Deep Learning capabilities

Architecture:

```python
spiral_model = Sequential()

spiral_model.add(Input(shape=(2,)))

spiral_model.add(layers.Dense(16, activation="relu"))
spiral_model.add(layers.Dense(16, activation="relu"))
spiral_model.add(layers.Dense(8, activation="relu"))

spiral_model.add(layers.Dense(1, activation="sigmoid"))
```

---

## 6. Regression with Neural Networks

Built a regression-oriented neural network using:

```python
activation="linear"
```

instead of sigmoid.

This allows the model to predict continuous numerical values.

Example:

```python
regression_model.add(layers.Dense(1, activation="linear"))
```

---

# Key Learnings

- Deep neural networks can learn highly complex patterns
- Activation functions are critical for non-linear learning
- Linear activation cannot solve non-linear classification tasks
- ReLU is an effective and commonly used activation function
- More complex datasets require deeper architectures

---

# TensorFlow Playground

Interactive playground used in this project:

https://playground.tensorflow.org/

---

# How to Run

Clone the repository:

```bash
git clone https://github.com/DPAMIR8781/S18D2-S-Data-playground.git
```

Go into the project directory:

```bash
cd S18D2-S-Data-playground
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
playground.ipynb
```

---

# Author

Doruk Pamir

Aspiring Data Analyst / Data Scientist
Focused on Machine Learning, Deep Learning, and Data Analytics
