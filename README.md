#  Plant Leaf Disease Classification (Tomato)

## Project Overview
This project focuses on classifying tomato leaf images into different disease categories using Convolutional Neural Networks (CNNs). The goal is to assist in early identification of plant diseases based on visual symptoms present on leaves.



---

##  Problem Statement
Manual identification of plant diseases is time-consuming and requires expert knowledge. An automated image-based classification system can help farmers and agricultural professionals quickly identify diseases and take preventive action.

---

##  Dataset
- **Source:** PlantVillage Dataset
- **Plant:** Tomato
- **Classes Used:**
  - Healthy
  - Early Blight
  - Late Blight
  - Leaf Mold


---

##  Methodology

### 1. Data Preparation
- Selected only tomato-related images from the dataset
- Organized images into class-wise folders
- Applied data augmentation to improve generalization

### 2. Model Architecture
- Base Model: **MobileNetV2** (pre-trained on ImageNet)
- Custom Classification Head:
  - Global Average Pooling
  - Dense Layer (ReLU)
  - Output Layer (Softmax for multi-class classification)

### 3. Training
- Image size: 224 × 224
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Train–Validation split: 80% / 20%

---

##  Results
The model achieved good validation accuracy and was able to correctly classify most tomato leaf images and model learned meaningful disease patterns.

---

## Limitations
- Occasional misclassification occurs between visually similar classes 
- Performance can be further improved with more diverse and larger datasets
- The model is intended for educational and experimental purposes

---

##  Technologies Used
- Python
- TensorFlow / Keras
- Google Colab
- GitHub
- Matplotlib

---
