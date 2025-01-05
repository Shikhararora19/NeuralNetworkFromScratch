# NeuralNetworkFromScratch 🚀

Welcome to **NeuralNetworkFromScratch**! 🎉 This project is a minimalist implementation of a Neural Network written in **Go** 🦦. It aims to teach the foundational concepts of neural networks while showcasing the power and simplicity of the Go programming language.

---

## 🌟 Features

- **Customizable Neural Network Architecture** 🧠
- **Support for CSV-based Training Data** 🗂️
- **Feedforward Neural Network Implementation** 🔁
- **Backward Propagation with Gradient Descent** 📉
- **Sigmoid Activation Function** ⚡
- **Matrix Operations using Gonum** 🧮
- Lightweight and modular codebase for experimentation ✨

---

## 🎯 Goals

1. **Learn the Basics of Neural Networks** 🏫
2. **Understand Mathematical Operations in NN** 🧾
3. **Leverage Go for Scientific Programming** 🛠️
4. **Provide a Hands-on Implementation for Beginners** 🎓

---

## 📖 Table of Contents

1. [Overview](#overview)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Code Structure](#code-structure)
5. [Examples](#examples)
6. [How It Works](#how-it-works)
7. [Roadmap](#roadmap)
8. [Contributing](#contributing)
9. [License](#license)

---

## 🧐 Overview

This project implements a basic feed-forward neural network with:

- Input Layer 🔍
- Hidden Layer 🌌
- Output Layer 🎯

The architecture and weights are designed for flexibility and experimentation. You can tweak parameters like the number of layers, neurons, activation functions, and learning rates.

---

## ⚙️ Installation

### Prerequisites

- **Go**: Install the Go programming language from [Go Downloads](https://golang.org/dl/).
- **gonum**: Install the Gonum library for matrix operations:
  ```bash
  go get -u gonum.org/v1/gonum/...
  ```

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/Shikhararora19/NeuralNetworkFromScratch.git
   cd NeuralNetworkFromScratch
   ```

2. Build the project:
   ```bash
   go build main.go
   ```

3. Run the executable:
   ```bash
   ./main
   ```

---

## 🚀 Usage

### Sample Run

1. Prepare your training and testing datasets in CSV format under the `data/` directory:
   - Training: `data/train.csv`
   - Testing: `data/test.csv`

2. Run the program:
   ```bash
   go run main.go
   ```

3. Observe the training progress and accuracy in the console output 📈.

### Example Configuration

The neural network is preconfigured with the following:
- **Input Neurons**: 4
- **Hidden Neurons**: 3
- **Output Neurons**: 3
- **Epochs**: 5000
- **Learning Rate**: 0.3

---

## 🧪 Examples

### Dataset Example

**Training Dataset (`data/train.csv`)**:
```csv
sepal_length,sepal_width,petal_length,petal_width,label_setosa,label_versicolor,label_virginica
5.1,3.5,1.4,0.2,1,0,0
4.9,3.0,1.4,0.2,1,0,0
6.2,3.4,5.4,2.3,0,0,1
5.9,3.0,5.1,1.8,0,1,0
```

### Training Output

```plaintext
Epoch 1: Loss = 1.23
Epoch 100: Loss = 0.85
Epoch 5000: Loss = 0.02

Accuracy = 0.95
```

---

## 🔍 How It Works

### 1. **Initialization**

- Random weights are assigned to each neuron connection.
- Biases are initialized to random values.

### 2. **Forward Propagation**

- Multiply inputs by weights.
- Add biases.
- Pass through activation functions (Sigmoid).

### 3. **Backward Propagation**

- Compute the error.
- Use gradients to adjust weights and biases.

### 4. **Training Loop**

- Repeat forward and backward propagation for several epochs.

---

## 🛣️ Roadmap

- [ ] Add support for more activation functions (ReLU, Tanh) 🔥
- [ ] Include support for additional datasets 📚
- [ ] Add performance benchmarks ⚡
- [ ] Extend to multi-layer networks ✨



---

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
