# Quantum Neural Network (QNN) Classifier – Two Moons Dataset

This repository contains a Python implementation of a **Variational Quantum Classifier** using PennyLane.  
The model is trained on the classical **two-moons dataset** and demonstrates how a shallow parameterized quantum circuit can perform binary classification.

---

## 📌 Overview

The project implements a 4-qubit **Discrete Variational Quantum Neural Network (QNN)** with:

- Angle encoding with feature duplication
- Two variational layers
- RZ–RY–RZ single-qubit rotations
- Ring entanglement (CNOT chain with wrap-around)
- Pauli-Z measurement for binary classification
- Binary cross-entropy loss
- Adam optimizer

The model learns to separate the nonlinearly separable two-moons dataset.

---

## 📊 Dataset

- Two-moons dataset
- 600 samples
- Noise = 0.15
- 75% training / 25% testing
- Features standardized before encoding

---

## ⚙️ Training Details

- Loss: Binary Cross-Entropy
- Optimizer: Adam
- Learning rate: 0.03
- Batch size: 64
- Training steps: 300
