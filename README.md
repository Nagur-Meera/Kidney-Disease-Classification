# Kidney Disease Classification  
**Using Digital Image Processing and Deep Learning**

This repository contains the implementation details, image processing pipeline, CNN model architecture, performance evaluation, and future roadmap for the project **Kidney Disease Classification**. The goal is to automate kidney disease detection from CT scan images using a combination of OpenCV-based preprocessing and deep learning-based classification.

📄 **Project Report:**  
🔗 [View Full Project Documentation](https://kidney-disease-classification.netlify.app/)

---

## 🧠 Project Overview

This project presents a medical image analysis system capable of classifying CT scan images into four kidney condition categories:

- **Normal**
- **Cyst**
- **Tumor**
- **Stone**

It achieves this through:
- Preprocessing raw images with digital image enhancement techniques
- Feeding the enhanced images into a custom-built CNN model
- Classifying them with **>90% accuracy** across all classes

---

## 🚀 Methodology

### 1. Digital Image Processing (OpenCV)
- **Resizing & Normalization**: Standardized to 224×224, pixel range [0,1]
- **CLAHE**: Contrast enhancement
- **Gaussian Blur**: Noise reduction
- **Laplacian/Sobel**: Edge detection

### 2. CNN-Based Classification (TensorFlow/Keras)
- 4 convolutional blocks (32 → 256 filters)
- Batch Normalization & Dropout layers
- Fully connected layer (512 units)
- Softmax output for 4-class prediction

---

## 🎯 Model Performance

| Metric         | Accuracy |
|----------------|----------|
| **Test Accuracy**   | 91.93%   |
| **Tumor**        | 94.17%   |
| **Cyst**         | 91.92%   |
| **Stone**        | 91.83%   |
| **Normal**       | 90.96%   |

---

## 📊 Dataset Summary

- **Total Images**: ~12,456
- **Split**: 70% Train / 15% Val / 15% Test
- **Class Distribution**:
  - Normal (40.8%)
  - Cyst (29.8%)
  - Tumor (18.4%)
  - Stone (11.1%)

---

## 🧪 Technologies Used

- **Image Processing**: OpenCV
- **Modeling**: TensorFlow, Keras
- **Visualization**: Matplotlib, Seaborn
- **Data Handling**: NumPy, Pandas
- **Reporting**: Netlify-hosted static site

---

## 🔬 Future Work

- Explore deeper architectures (ResNet, DenseNet)
- Apply Grad-CAM for interpretability
- Improve class balance via augmentation
- Add clinical validation with larger datasets


