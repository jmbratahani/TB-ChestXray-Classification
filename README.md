
# TB-ChestXray-Classification-Deep-Learning-Project

A deep learning project classifying Tuberculosis (TB) vs. normal chest X-ray images using Convolutional Neural Networks (CNNs), transfer learning, and dropout regularization to achieve high accuracy. This repository aims to help automate and enhance TB screening, especially in resource-limited settings where experienced radiologists may not be readily available.

---

## Project Overview

Tuberculosis (TB) is a leading cause of death from a single infectious agent, yet it’s treatable when diagnosed early. Traditional chest X-ray reading by radiologists can be time-consuming and prone to variability, especially in regions with fewer specialists. Deep learning approaches, specifically CNNs, can assist in diagnosing TB effectively by automating the identification of TB-positive X-ray scans.

**Key Objectives:**

- Automate classification of normal vs. TB-positive chest X-rays.  
- Compare and evaluate various deep learning architectures.  
- Provide a tool that can assist healthcare professionals in TB screening.

---

## Dataset

- **Source:** Chest X-ray images sourced from Tuberculosis (TB) Chest X-ray Database [Kaggle](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset?resource=download)
- **Composition:** 
  - 3,500 normal chest X-ray images  
  - 700 TB-positive chest X-ray images  

---

## Approaches

### 1. Deep Neural Networks (DNN)
- Explored 1 to 4 hidden layers.
- Used ReLU activation and a final sigmoid for binary classification.
- Achieved a validation accuracy of around **0.958**.


### 2. CNN Architectures
- **CNN without Dropout**: Achieved **0.991** validation accuracy.
- **CNN with Dropout**: Achieved **0.996** validation accuracy (best performance in our experiments).

### 3. Transfer Learning
- **Inception V3** and **DenseNet201** pre-trained on ImageNet.
- Added custom layers (Flatten or GlobalAveragePooling, Dropout, etc.).
- Validation accuracies up to **0.994 (InceptionV3)** and **0.995 (DenseNet201)**.

---

## Results

- **Best Model**: CNN with a Dropout layer before the final layer.
- **Highest Validation Accuracy**: 0.996.
- This indicates a strong performance in distinguishing TB from normal chest X-rays.

---
## Contributors

This project was completed as a final project for **DSO 569 - Deep Learning** graduate course at **USC Marshall School of Business**

[Katsuhiko Adachi]
[Jessica Bratahani]
[Pin-Hsuan Chang]
[Teresa Chen]
[Jesslyn Noorjono]

