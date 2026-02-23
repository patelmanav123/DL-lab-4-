# Lab 4: Single Layer Perceptron & Multi-Layer Perceptron (MLP)

## 📘 Overview
This lab demonstrates the implementation of:

- **Single Layer Perceptron (SLP)** from scratch  
- **Multi-Layer Perceptron (MLP)** using NumPy  

The goal is to understand how neural networks learn **linear** vs **non-linear** decision boundaries.

---

## 🎯 Objectives

✔ Implement a perceptron using first principles  
✔ Train a model on synthetic data  
✔ Build an MLP capable of solving XOR  
✔ Compare linear vs non-linear learning  
✔ Analyze the impact of hidden layer size  
✔ Visualize decision boundaries and loss curves  

---

## 🧠 Task 1: Single Layer Perceptron

### Description
A perceptron is trained to classify 2D points using a **linear decision boundary**.

### Key Steps
- Generate synthetic dataset
- Define perceptron function
- Train using perceptron learning rule
- Plot decision boundary

### Limitation
❌ Cannot solve non-linear problems (e.g., XOR)

---

## 🔥 Task 2: Multi-Layer Perceptron (MLP)

### Description
An MLP with:

- **Input Layer:** 2 neurons  
- **Hidden Layer:** 4 neurons (ReLU)  
- **Output Layer:** 1 neuron (Sigmoid)

is implemented to learn **non-linear patterns**.

### Key Steps
- Initialize weights & biases
- Forward propagation
- Backpropagation
- Train on XOR dataset

### Capability
✔ Successfully solves XOR

---

## 📊 Task 3: Experiments & Analysis

### 1️⃣ Perceptron vs MLP

| Model | Linear Data | XOR Data |
|------|-------------|----------|
| Perceptron | ✅ 100% Accuracy | ❌ 50% Accuracy |
| MLP | ✅ Learns | ✅ Learns |

---

### 2️⃣ Hidden Layer Size Impact

| Hidden Neurons | Final Loss |
|---------------|------------|
| 2 | 0.6931 (Underfitting) |
| 4 | 0.0015 (Good Learning) |
| 8 | 0.0035 |

✔ Moderate hidden size performs best

---

### 3️⃣ Loss Curve Observation

- High loss at start  
- Gradual decrease  
- Stable minimum  

✔ Indicates successful training

---

## ⚙️ Technologies Used

- Python  
- NumPy  
- Matplotlib  

---

## ▶️ How to Run

1. Install dependencies:
   ```bash
   pip install numpy matplotlib
