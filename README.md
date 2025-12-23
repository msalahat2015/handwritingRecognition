# Handwritten Digit Classification Using CNNs

This repository implements and compares multiple Convolutional Neural Network (CNN) architectures for handwritten digit classification. The models are trained and evaluated using the **Arabic Handwritten Digits Dataset (AHDD)**.

---

## 📁 Dataset Preparation

### AHDD Dataset
- Loaded from Google Drive in CSV format.
- Each image is reshaped from a 784-dimensional vector to a 28×28 grayscale image.
- Pixel values are normalized to the range [0, 1].
- A custom PyTorch `Dataset` and `DataLoader` are used for efficient batching.



---

## 🧠 Models Implemented

### 1️⃣ AlexNet
- Modified to accept single-channel grayscale images.
- Deep convolutional architecture for hierarchical feature extraction.
- Fully connected layers perform digit classification.
- Trained using Adam optimizer and evaluated with accuracy, F1-score, and a normalized confusion matrix.

### 2️⃣ LeNet
- Classical CNN architecture designed for digit recognition.
- Uses convolution, ReLU activation, and average pooling.
- Lightweight and efficient, serving as a baseline model.
- Performance evaluated using accuracy, F1-score, and confusion matrix.

### 3️⃣ Custom CNN
- Deeper and more flexible CNN architecture.
- Uses convolutional blocks with batch normalization, ReLU, and max pooling.
- Applies global average pooling for compact feature representation.
- Designed to enhance feature learning and classification performance.

---

## ⚙️ Training Configuration

- **Loss Function:** Cross-Entropy Loss  
- **Optimizer:** Adam  
- **Batch Size:** 64  
- **Epochs:** 10  

All models are trained using supervised learning and evaluated on a separate test set.

---

## 📊 Evaluation Metrics

- Classification Accuracy  
- Macro F1-score  
- Normalized Confusion Matrix (saved as high-resolution images)

---

## 📌 Outputs

- Trained CNN models
- Training loss per epoch
- Test accuracy and F1-score
- Normalized confusion matrix visualizations for each model

---

## 🚀 Conclusion

This project demonstrates and compares the effectiveness of classical, deep, and custom-designed CNN architectures for handwritten digit recognition, highlighting their performance and architectural differences.

---
