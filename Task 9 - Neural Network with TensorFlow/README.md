# 🧠 Advanced Task 3: Neural Network for MNIST Digit Classification

## 📌 Task Overview

**Level:** Advanced  
**Task:** Build and train a simple feed-forward neural network using TensorFlow/Keras to classify handwritten digits from the MNIST dataset.

---

## 🎯 Objectives

- Load and preprocess the MNIST dataset.
- Design a multi-layer feed-forward neural network using TensorFlow/Keras.
- Train the model using backpropagation and monitor performance.
- Evaluate the model on test data.
- Visualize training and validation accuracy and loss across epochs.

---

## 🛠️ Tools & Libraries

- Python
- TensorFlow / Keras
- Matplotlib
- NumPy (implicitly used through TensorFlow)

---

## 🧪 Dataset Details

- **Source:** `tensorflow.keras.datasets.mnist`
- **Size:** 60,000 training samples + 10,000 test samples
- **Classes:** 10 digits (0 through 9)
- **Input Shape:** 28×28 pixels (flattened to 784 features)

---

## 🏗️ Model Architecture

| Layer Type | Units | Activation |
|------------|-------|------------|
| Dense (Input) | 128 | ReLU |
| Dense | 64 | ReLU |
| Dense (Output) | 10 | Softmax |

---

## ⚙️ Training Details

- **Optimizer:** Adam  
- **Loss Function:** Categorical Crossentropy  
- **Metrics:** Accuracy  
- **Epochs:** 10  
- **Batch Size:** 128  
- **Validation Split:** 20% from training set

---

## 📊 Results Summary

- The model successfully learned to classify handwritten digits.
- It achieved high training and validation accuracy within a small number of epochs.
- Visualization shows steady improvement in both training and validation accuracy and a decrease in loss, indicating proper convergence.

### ✔ Final Test Accuracy

Achieved **~97.7% accuracy** on the test dataset.

---

## 📈 Visualizations

Two plots were generated:

1. **Training & Validation Accuracy**  
2. **Training & Validation Loss**  

These help monitor overfitting or underfitting during training.

---
