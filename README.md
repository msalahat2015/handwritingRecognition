Handwritten Digit Classification Using CNNs

This project implements and compares multiple Convolutional Neural Network (CNN) architectures for handwritten digit classification. The models are trained and evaluated using the Arabic Handwritten Digits Dataset (AHDD) and the MNIST dataset.

📁 Dataset Preparation
AHDD Dataset

Loaded from Google Drive in CSV format.

Each image is reshaped from a 784-dimensional vector to a 28×28 grayscale image.

Pixel values are normalized to the range 
[0,1]
[0,1].

Images are resized to 227×227 to match AlexNet input requirements.

A custom PyTorch Dataset and DataLoader are used for efficient batching and training.

MNIST Dataset

Downloaded directly using torchvision.datasets.

Images are converted to tensors and normalized.

Used for training and testing LeNet and the Custom CNN models.

🧠 Models Implemented
1️⃣ AlexNet

Adapted to accept single-channel grayscale images.

Deep convolutional architecture for hierarchical feature extraction.

Fully connected layers perform digit classification.

Optimized using Adam and evaluated with accuracy, F1-score, and a normalized confusion matrix.

2️⃣ LeNet

Classical CNN architecture designed for digit recognition.

Uses convolution, ReLU activation, and average pooling.

Lightweight and efficient for baseline performance comparison.

Evaluation includes accuracy, F1-score, and confusion matrix visualization.

3️⃣ Custom CNN

Designed with multiple convolutional blocks.

Incorporates batch normalization, ReLU activation, and max pooling.

Uses global average pooling for compact feature representation.

Provides improved feature learning and robust classification performance.

⚙️ Training & Optimization

Loss Function: Cross-Entropy Loss

Optimizer: Adam

Batch Size: 64

Epochs: 10

Each model is trained using supervised learning and evaluated on a separate test set.

📊 Evaluation Metrics

Classification Accuracy

Macro F1-score

Normalized Confusion Matrix (saved as high-resolution images)

📌 Output

Trained CNN models

Printed training loss per epoch

Accuracy and F1-score results

Confusion matrix visualizations for each model

🚀 Conclusion

This project demonstrates the effectiveness of different CNN architectures for handwritten digit recognition, highlighting the trade-offs between classical, deep, and custom-designed networks.
