# MVC Project — Multilayer Perceptron
**Roll Number:** i253029  
**Course:** Artificial Neural Networks  
**University:** National University of Computer and Emerging Sciences (FAST-NUCES)

---

## Project Overview

Manual and programmatic implementation of a Multilayer Perceptron (MLP) from scratch.  
Tasks 1–6 are performed manually on a 3-sample student performance dataset.  
Task 7 scales the implementation to MNIST using NumPy only (no PyTorch/TensorFlow).

---

## Network Architecture

| Layer   | Type           | Neurons | Activation |
|---------|----------------|---------|------------|
| Layer 0 | Input          | 784     | —          |
| Layer 1 | Hidden Layer 1 | 128     | Sigmoid    |
| Layer 2 | Hidden Layer 2 | 64      | Sigmoid    |
| Layer 3 | Output         | 10      | Sigmoid    |

---

## Repository Structure

```
mvc-mlp-i253029/
├── src/
│   └── mlp_mnist_i253029.ipynb   ← Jupyter Notebook (Task 7)
├── data/
│   └── mnist.npz                 ← MNIST dataset (auto-downloaded)
├── report/
│   ├── report_i253029.pdf        ← LaTeX report (Task 8)
│  
│   
└── README.md
```

---

## How to Run

### Prerequisites
```bash
pip install numpy matplotlib jupyter
```

### Step 1 — Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/mvc-mlp-i253029.git
cd mvc-mlp-i253029
```

### Step 2 — Run the notebook
```bash
jupyter notebook src/mlp_mnist_i253029.ipynb
```
Then select **Kernel → Restart & Run All**.

The notebook will:
1. Train the MLP for 20 epochs
2. Print test accuracy

---

## Training Configuration

| Hyperparameter    | Value  |
|-------------------|--------|
| Learning rate (η) | 0.1    |
| Batch size (B)    | 32     |
| Epochs            | 20     |
| Loss function     | MSE    |
| Optimiser         | Mini-Batch GD |
| Weight init       | Uniform(-0.5, 0.5) |
| Random seed       | 42     |


## Weights Used (Manual Tasks 1–6)

| Parameter | Value |
|-----------|-------|
| w1  |  0.33 | w2  | -0.38 |
| w3  | -0.03 | w4  | -0.34 |
| w5  | -0.38 | w6  |  0.74 |
| w7  |  0.08 | w8  |  0.18 |
| w9  | -0.42 | w10 |  0.33 |
| b¹  |  0.16 | b²  |  0.04 |
