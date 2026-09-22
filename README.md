# 🧠 Brain Tumor Detection Using CNN

A deep learning-based **Brain Tumor Detection system** that uses **Convolutional Neural Networks (CNN)** to classify brain MRI images into **Tumor** and **No Tumor** categories. The project demonstrates how deep learning and computer vision can be applied to medical image classification and preliminary screening.

## 🚀 Project Overview

Brain tumor detection from MRI scans requires careful analysis of medical images. This project aims to automate the **initial classification of brain MRI images** using a CNN model that learns visual patterns and features directly from the images.

The system takes an MRI image as input, processes it, and predicts whether the image belongs to the **Tumor** or **No Tumor** class.

> **Note:** This is an academic deep learning project and is intended for research and educational purposes. It is not a substitute for professional medical diagnosis.

## 🌟 Features

* 🧠 CNN-based brain MRI image classification
* 🔍 Tumor vs. No Tumor prediction
* 🖼️ Automated image preprocessing
* 📊 Model performance evaluation
* 📈 Accuracy, Precision, Recall, and F1-score analysis
* 📉 Confusion matrix visualization
* 🛡️ Dropout-based overfitting reduction
* ⚡ Adam optimizer for model training

## 🛠️ Tech Stack

### Programming Language

* Python

### Machine Learning & Deep Learning

* TensorFlow
* Keras
* Scikit-learn

### Image Processing & Data Analysis

* OpenCV
* PIL
* NumPy
* Pandas
* Matplotlib

## 🔄 How It Works

```text
MRI Image
    ↓
Image Preprocessing
    ↓
Resize to 64 × 64
    ↓
Convert Image to Numerical Array
    ↓
CNN Feature Extraction
    ↓
Pooling & Dropout
    ↓
Dense Classification Layer
    ↓
Tumor / No Tumor Prediction
```

## 🧪 Data Preprocessing

The MRI dataset is organized into two categories:

```text
datasets/
├── no/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── ...
│
└── yes/
    ├── image1.jpg
    ├── image2.jpg
    └── ...
```

The images are:

* Loaded using OpenCV/PIL
* Resized to **64 × 64 pixels**
* Converted into numerical arrays
* Assigned binary labels:

  * `0` → No Tumor
  * `1` → Tumor
* Split into training and testing datasets

## 🧠 CNN Architecture

The model follows a Sequential CNN architecture consisting of:

* **Conv2D** — extracts important visual features from MRI images
* **MaxPooling2D** — reduces spatial dimensions and computational complexity
* **Dropout** — helps reduce overfitting
* **Flatten** — converts extracted feature maps into a one-dimensional vector
* **Dense Layers** — perform classification
* **Output Layer** — produces the final tumor/no-tumor prediction

### Training Configuration

* **Optimizer:** Adam
* **Loss Function:** Binary Cross-Entropy
* **Classification:** Binary
* **Input Size:** 64 × 64 × 3

## 📊 Model Evaluation

The model performance is evaluated using multiple classification metrics:

| Metric           | Purpose                                          |
| ---------------- | ------------------------------------------------ |
| Accuracy         | Measures overall correct predictions             |
| Precision        | Measures the correctness of positive predictions |
| Recall           | Measures the ability to identify positive cases  |
| F1-Score         | Provides a balance between precision and recall  |
| Confusion Matrix | Shows correct and incorrect classifications      |

## 🎯 Problem Solved

The project demonstrates an automated approach for **preliminary classification of brain MRI images**, reducing the need for manually inspecting every image during an initial screening process.

By using CNN-based feature extraction, the system can learn relevant patterns from MRI images and classify them into tumor and non-tumor categories.

## 📂 Project Structure

```text
Brain-Tumor-Detection/
│
├── datasets/
│   ├── yes/
│   └── no/
│
├── notebooks/
│
├── model/
│
├── results/
│
├── main.py
├── requirements.txt
└── README.md
```

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/brain-tumor-detection.git
cd brain-tumor-detection
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Project

```bash
python main.py
```

## 📦 Requirements

```text
tensorflow
keras
opencv-python
numpy
pandas
matplotlib
scikit-learn
Pillow
```

## 🔮 Future Enhancements

* Improve classification performance with a larger and more diverse dataset
* Implement **Transfer Learning** using models such as ResNet or EfficientNet
* Add a web interface for uploading MRI images
* Deploy the model as a web application
* Add explainable AI techniques such as **Grad-CAM**
* Provide confidence scores with predictions
* Explore multi-class brain tumor classification

## 👨‍💻 Developer

**Ambuj Yadav**

* GitHub: https://github.com/ydv-ambuj
* LinkedIn: https://www.linkedin.com/in/ambuj-yadav-000188380
* Email: [ambujyadav1984@gmail.com](mailto:ambujyadav1984@gmail.com)

## 📜 License

This project is licensed under the **MIT License**.
