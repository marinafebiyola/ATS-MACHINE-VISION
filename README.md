# ATS-MACHINE-VISION
This repository is for store the program 
# EMNIST Handwritten Letter Classification using HOG + SVM

This project classifies handwritten letters from the EMNIST Letters Dataset
using Histogram of Oriented Gradients (HOG) feature extraction and
**Support Vector Machine (SVM)** classifier.

---

## 👩‍💻 Author
Name: Marina Febiyola Br Tarigan  
NIM: 4212301021  
Class: MK5A Pagi  

---

## 🎯 Objective
Implement machine learning to classify 26 handwritten alphabet letters (A–Z)
from the EMNIST dataset using feature-based methods (HOG) and Support Vector Machine.

---

## 🧠 Method Overview

### 1. Data Preprocessing
- Load dataset `emnist-letters-train.csv`
- Select 500 samples per class → total 13,000 samples
- Normalize pixel values to [0,1]
- Reshape to 28×28 images

### 2. Feature Extraction (HOG)
- Extract HOG features with orientations = 9, pixel cell = (8,8), block = (2,2)
- HOG captures edge and shape information useful for letter recognition

### 3. Classification (SVM)
- Use Support Vector Machine with RBF kernel
- Parameters: `C=10`, `gamma=0.01`

### 4. Evaluation (LOOCV)
- Evaluate model using **Leave-One-Out Cross Validation**
- Metrics: Accuracy, Precision, Recall, F1-score
- Show confusion matrix

### 5. Parameter Tuning
- Try several HOG and SVM parameter combinations
- Select best accuracy combination
