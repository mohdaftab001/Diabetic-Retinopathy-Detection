# Diabetic-Retinopathy-Detection
AI Based Diabetic Retinopathy Detection System
# 🩺 AI-Based Diabetic Retinopathy Detection System using Swin Transformer


![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red)
![TorchVision](https://img.shields.io/badge/TorchVision-Computer%20Vision-green)
![OpenCV](https://img.shields.io/badge/OpenCV-Image%20Processing-blue)
![Swin%20Transformer](https://img.shields.io/badge/Swin%20Transformer-Vision%20Transformer-purple)
![Gradio](https://img.shields.io/badge/Gradio-Deployment-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)


## 📖 Overview

Diabetic Retinopathy (DR) is one of the leading causes of preventable blindness among diabetic patients. Early detection is essential because timely treatment can significantly reduce the risk of vision loss.

This project presents an AI-powered automated screening system that detects and classifies Diabetic Retinopathy from retinal fundus images using Deep Learning and Computer Vision techniques.

The system utilizes a Swin Transformer architecture to analyze retinal images and classify them into five severity levels. It also provides prediction confidence and clinical recommendations, making it a useful decision-support tool for healthcare professionals.

---

## 🎯 Problem Statement

Traditional diabetic retinopathy screening faces several challenges:

- Requires trained ophthalmologists
- Manual examination is time-consuming
- High screening costs
- Limited accessibility in rural areas
- Delayed diagnosis can lead to permanent blindness

This project aims to address these challenges by providing an automated AI-based screening solution.

---

## 🎯 Objectives

- Detect Diabetic Retinopathy automatically from retinal fundus images
- Classify disease severity into five categories
- Reduce diagnosis time
- Assist healthcare professionals in screening
- Improve accessibility of eye care services
- Build a deployable AI-powered healthcare solution

---

## 🏥 Diabetic Retinopathy Severity Levels

| Class | Severity Level |
|---------|---------|
| 0 | No DR |
| 1 | Mild |
| 2 | Moderate |
| 3 | Severe |
| 4 | Proliferative DR |

---

## 📊 Dataset

### Dataset Used
- APTOS 2019 Blindness Detection Dataset

### Dataset Features
- Retinal Fundus Images
- Multiple Disease Severity Levels
- Real-world Medical Image Variations
- Imbalanced Class Distribution

### Dataset Challenges
- Uneven class distribution
- Image quality variations
- Different illumination conditions
- Noise and blur

---

## ⚙️ Data Preprocessing

To improve model performance, several preprocessing techniques were applied:

### Image Resizing
All images were resized to:

```python
224 × 224
```

### RGB Conversion
Images were converted into RGB format for consistent feature extraction.

### Normalization
Pixel values were normalized to improve training stability and convergence.

### Data Augmentation
Applied techniques include:

- Rotation
- Horizontal Flip
- Vertical Flip
- Brightness Adjustment
- Zoom Transformations

### Benefits
- Reduces overfitting
- Improves model generalization
- Increases dataset diversity

---

## 🤖 Models Explored

### 1. Convolutional Neural Network (CNN)

CNN is a deep learning architecture specifically designed for image processing.

**Advantages**
- Learns image features automatically
- Detects textures, edges, and patterns
- Effective for computer vision tasks

---

### 2. EfficientNet

EfficientNet is an optimized CNN architecture that balances:

- Network depth
- Width
- Image resolution

**Advantages**
- High accuracy
- Fewer parameters
- Computational efficiency

---

### 3. Swin Transformer (Final Model)

The final implementation uses Swin Transformer.

#### Why Swin Transformer?

Unlike traditional CNNs, Swin Transformer uses a Self-Attention Mechanism that allows the model to:

- Capture local retinal features
- Understand global image relationships
- Learn complex disease patterns
- Improve feature representation

#### Key Innovation

**Shifted Window Attention**

This mechanism enables efficient learning while maintaining computational efficiency.

---

## 🏗️ System Architecture

```text
Retinal Fundus Image
        │
        ▼
Data Preprocessing
        │
        ▼
Feature Extraction
        │
        ▼
Swin Transformer
        │
        ▼
Softmax Classification
        │
        ▼
DR Severity Prediction
        │
        ▼
Clinical Recommendation
```

---

## 🔧 Technologies Used

### Programming Language
- Python

### Deep Learning
- PyTorch
- TorchVision

### Computer Vision
- OpenCV

### Data Processing
- NumPy
- Pandas

### Visualization
- Matplotlib
- Seaborn

### Deployment
- Gradio

---

## 📈 Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Sensitivity
- Specificity
- ROC-AUC Score
- Confusion Matrix

---

## ✨ Features

- ✅ Automated DR Detection
- ✅ Five-Class Classification
- ✅ Real-Time Prediction
- ✅ Confidence Score Generation
- ✅ Probability Visualization
- ✅ AI-Based Clinical Recommendation
- ✅ User-Friendly Gradio Interface

---

## 🚧 Challenges Faced

### Dataset Imbalance
The dataset contained significantly more normal cases compared to severe cases.

### Prediction Bias
Some classes received fewer predictions due to class imbalance.

### Medical Image Variability
Retinal images varied in:
- Brightness
- Contrast
- Resolution
- Noise Levels

### Model Generalization
Ensuring consistent performance across diverse retinal images was challenging.

---

## 💡 Project Highlights

- Swin Transformer implementation for retinal image analysis
- Attention-based feature learning
- AI-assisted healthcare screening workflow
- Clinical recommendation system
- Real-time prediction interface
- Automated severity classification

---

## 🔮 Future Scope

- Mobile Application Deployment
- Cloud-Based Healthcare Platform
- Explainable AI (Grad-CAM Heatmaps)
- Integration with OCT Imaging
- Electronic Health Record (EHR) Integration
- Larger Multi-Hospital Datasets
- Improved Class Balancing Techniques

---

## 🌍 Real-World Impact

This system can:

- Assist ophthalmologists in diagnosis
- Reduce screening workload
- Enable faster disease detection
- Improve healthcare accessibility
- Help prevent diabetes-related blindness

---

## 👨‍💻 Author

**Mohd Aaftab**  
B.Tech (Artificial Intelligence)  
NIET, Greater Noida

---

