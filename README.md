# SVM – Breast Cancer Classification

## 📌 Overview
This project implements a **Support Vector Machine (SVM)** model to classify breast cancer tumors as **Malignant** or **Benign** using the **Scikit-learn Breast Cancer Dataset**.  
The objective is to understand **kernel-based classification**, **feature scaling**, and **hyperparameter tuning**.

---

## 📊 Dataset
- **Source:** Scikit-learn (`load_breast_cancer`)
- **Samples:** 569
- **Features:** 30 numeric features
- **Target Classes:**
  - `0` → Malignant
  - `1` → Benign

---

## 🛠 Tools & Libraries
- Python
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- Joblib

---

## ⚙️ Methodology
1. Loaded and explored the breast cancer dataset
2. Performed train-test split
3. Applied **StandardScaler** for feature normalization
4. Trained baseline SVM with **Linear Kernel**
5. Trained SVM with **RBF Kernel**
6. Tuned hyperparameters (`C`, `gamma`) using **GridSearchCV**
7. Evaluated the best model using:
   - Accuracy
   - Confusion Matrix
   - Classification Report
   - ROC Curve & AUC
8. Saved the final trained pipeline (Scaler + SVM)

---

## 📈 Model Performance

### Test Accuracy
**98.24%**

### Confusion Matrix

### Classification Report
- Precision, Recall, and F1-score are **above 0.98** for both classes
- Only **2 misclassifications** out of 114 test samples

### ROC & AUC
- ROC Curve plotted for visual evaluation
- High AUC score indicates excellent class separability

---

## 💾 Saved Model
The tuned SVM model pipeline is saved using Joblib:
This file includes both **StandardScaler** and **SVM classifier** for direct reuse.

---


---

## 🎯 Learning Outcome
- Understanding of **SVM margin and kernels**
- Importance of **feature scaling**
- Hands-on experience with **hyperparameter tuning**
- Evaluation of medical classification models

---

## 🧠 Key Concepts
- Linear vs RBF Kernel
- Regularization parameter (C)
- Gamma parameter
- ROC Curve & AUC

