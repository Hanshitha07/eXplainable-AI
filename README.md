# 🌱 Plant Disease Detection Using Multimodal Deep Learning with Explainable AI

> 🚧 Ongoing Research & Development Project

## 📌 Overview

Plant diseases significantly affect crop yield and agricultural productivity. Early disease detection can help farmers take preventive measures and reduce losses.

This project aims to develop an Explainable AI (XAI) based plant disease detection system using Deep Learning techniques. The system analyzes plant leaf images, identifies diseases, and provides visual explanations for its predictions to improve transparency and trustworthiness.

Unlike traditional black-box AI models, this project integrates Explainable AI methods such as LIME, SHAP, and Grad-CAM to help users understand why a particular prediction was made.

This is currently an ongoing project under active development, and additional features, datasets, and multimodal capabilities will be integrated in future phases.

---

# 🎯 Objectives

- Detect plant diseases from leaf images using Deep Learning.
- Classify tomato leaf diseases accurately.
- Improve model transparency through Explainable AI techniques.
- Visualize regions influencing model predictions.
- Develop a trustworthy and interpretable AI system.
- Build the foundation for a future multimodal disease diagnosis platform.

---

# 🦠 Current Disease Classes

The current implementation focuses on Tomato Leaf Diseases:

| Class | Description |
|---------|------------|
| 🍃 Healthy | Healthy Tomato Leaf |
| 🟠 Early Blight | Fungal disease causing brown lesions |
| 🔴 Late Blight | Severe disease affecting leaves and stems |

---

# 📂 Dataset

### Dataset Used
PlantVillage Dataset (Kaggle)

### Current Dataset Scope
- Tomato Healthy
- Tomato Early Blight
- Tomato Late Blight

### Preprocessing Steps
- Image resizing (224 × 224)
- Pixel normalization
- Train-validation split
- Data augmentation

---

# 🧠 Deep Learning Model

### Model Architecture
- MobileNetV2 (Transfer Learning)

### Frameworks
- TensorFlow
- Keras

### Training Strategy
- Feature extraction using pretrained MobileNetV2
- Custom classification layers
- Fine-tuning of upper layers
- Early stopping and checkpointing

### Output
The model predicts:
- Disease Class
- Prediction Confidence Score

Example:

```text
Disease    : Tomato Early Blight
Confidence : 99.0%
```

---

# 🔍 Explainable AI (XAI)

One of the primary goals of this project is to improve model interpretability.

## 1️⃣ LIME (Local Interpretable Model-Agnostic Explanations)

LIME explains individual predictions by identifying image regions that contributed to the final decision.

### Interpretation

🟢 Green Regions
- Support the predicted class

🔴 Red Regions
- Oppose the predicted class

### Purpose

Helps visualize which infected regions influenced the model's decision.

---

## 2️⃣ SHAP (SHapley Additive exPlanations)

SHAP calculates the contribution of image features toward each prediction.

### Interpretation

🔴 Red Regions
- Increase prediction confidence

🔵 Blue Regions
- Decrease prediction confidence

### Outputs

- SHAP Attribution Maps
- SHAP Feature Importance Graphs
- SHAP Overlay Visualizations

### Purpose

Provides both local and global explanations for model behavior.

---

## 3️⃣ Grad-CAM

Grad-CAM generates heatmaps showing where the neural network focuses before making a prediction.

### Interpretation

🔴 Red / Yellow Regions
- Highly important regions

🔵 Blue Regions
- Less important regions

### Purpose

Visual verification of disease localization.

---

# 📊 Current Progress

## ✅ Completed Work

- Dataset collection and preprocessing
- Tomato disease dataset preparation
- Deep learning model development
- MobileNetV2 implementation
- Model training and validation
- Disease prediction system
- Confidence score generation
- LIME integration
- SHAP integration
- Grad-CAM integration
- Prediction visualization
- Performance evaluation

---

# 📈 Sample Outputs

### Disease Prediction

```text
Tomato Early Blight
Confidence: 99%
```

### Generated Visualizations

- Class Distribution Graph
- Sample Dataset Visualization
- Confusion Matrix
- Prediction Confidence Graph
- LIME Explanation Maps
- SHAP Attribution Maps
- SHAP Feature Importance Graphs
- Grad-CAM Heatmaps

---

# 🛠️ Tech Stack

## Programming Language

- Python

## Deep Learning

- TensorFlow
- Keras

## Explainable AI

- LIME
- SHAP
- Grad-CAM

## Data Processing

- NumPy
- OpenCV

## Visualization

- Matplotlib
- Seaborn

## Development Environment

- Google Colab

---

# 📁 Project Structure

```text
Plant-Disease-Detection-XAI/
│
├── dataset/
│
├── notebooks/
│   ├── data_preprocessing.ipynb
│   ├── model_training.ipynb
│   ├── prediction.ipynb
│   ├── lime_explanation.ipynb
│   ├── shap_explanation.ipynb
│   └── gradcam.ipynb
│
├── models/
│   ├── best_model.h5
│   └── plant_disease_model_final.h5
│
├── outputs/
│   ├── confusion_matrix.png
│   ├── prediction_result.png
│   ├── lime_explanation.png
│   ├── shap_importance.png
│   ├── shap_overlay.png
│   └── gradcam_result.png
│
└── README.md
```

---

# 🚀 Future Work (OpenLab Phase-1)

The project is still under active development.

Upcoming work includes:

### 🔄 Model Improvements

- Improve classification accuracy
- Hyperparameter optimization
- Advanced fine-tuning

### 🌱 Dataset Expansion

- Additional plant species
- Additional disease classes
- Real-world field images

### 🧩 Multimodal AI Integration

- Image + Text based diagnosis
- Disease description understanding
- Symptom-based prediction support

### 🌍 Deployment

- Web Application
- Farmer-friendly user interface
- Real-time prediction system

### 🔬 Advanced Explainability

- Improved SHAP visualizations
- Better disease localization
- Comparative XAI analysis

### 📱 Future Extensions

- Mobile application support
- Cloud deployment
- Edge AI implementation

---

# ⚠️ Project Status

```diff
+ Current Status : Ongoing Development
```

This repository represents the current progress of our Explainable AI-based Plant Disease Detection project.

Several components have been successfully implemented; however, many advanced features and multimodal capabilities are still under development.

The repository will be continuously updated as new experiments, models, datasets, and explainability techniques are integrated.

---

# 👨‍💻 Authors

OpenLab Research Project

Plant Disease Detection Using Multimodal Deep Learning with Explainable AI

---

# ⭐ Acknowledgements

- PlantVillage Dataset
- TensorFlow & Keras
- LIME
- SHAP
- Google Colab
- Open Source AI Community
