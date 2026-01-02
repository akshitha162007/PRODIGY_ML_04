
#  Hand Gesture Recognition using Machine Learning

##  Project Overview

This project implements a **Hand Gesture Recognition system** that classifies different hand gestures from image data. The goal is to enable **gesture-based human–computer interaction**, allowing users to control systems using hand movements instead of traditional input devices.

The project uses the **LeapGestRecog dataset** and applies a **machine learning approach** for multi-class gesture classification.

---

##  Objectives

* To load and preprocess hand gesture images
* To extract meaningful numerical representations from images
* To train a machine learning model capable of recognizing hand gestures
* To evaluate the model using standard classification metrics

---

##  Dataset Description

* **Dataset Name:** LeapGestRecog
* **Source:** Kaggle
* **Link:** [https://www.kaggle.com/gti-upm/leapgestrecog](https://www.kaggle.com/gti-upm/leapgestrecog)

### Dataset Structure

```
leapGestRecog/
├── 00/
│   ├── 01_palm
│   ├── 02_l
│   ├── 03_fist
│   ├── 04_fist_moved
│   ├── 05_thumb
│   ├── 06_index
│   ├── 07_ok
│   ├── 08_palm_moved
│   ├── 09_c
│   └── 10_down
├── 01/
├── 02/
└── ...
```

* Each numbered folder represents a different subject.
* Each subfolder corresponds to a **unique hand gesture class**.
* Images are grayscale, simplifying preprocessing.

---

##  Methodology

### 1. Image Preprocessing

* Images are resized to **64×64 pixels**
* Each image is converted into a **1D feature vector** by flattening pixel values
* This ensures consistent input size for the model

### 2. Feature Representation

* Raw pixel values are used as features
* This approach keeps the model simple and easy to understand

### 3. Model Used

* **Support Vector Machine (SVM)**
* Kernel: Linear
* SVM was chosen because it performs well for classification tasks with structured input data and limited samples

---

##  Workflow

```
Image Dataset
   ↓
Image Resizing & Flattening
   ↓
Train–Test Split
   ↓
SVM Model Training
   ↓
Gesture Classification
   ↓
Performance Evaluation
```

---

##  Technologies Used

* Python
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib (optional, for visualization)

---

##  Model Evaluation

The model performance is evaluated using:

* **Accuracy Score**
* **Precision, Recall, and F1-score** (Classification Report)

 **Note:**
The accuracy varies depending on:

* Number of images used per gesture
* Train–test split
* Image selection order

This variation is **expected and normal** in machine learning projects.

---

##  Applications

* Gesture-based user interfaces
* Touchless control systems
* Human–computer interaction
* Assistive technologies
* Smart devices and automation

---

##  Conclusion

This project demonstrates how machine learning techniques can be applied to recognize hand gestures from image data. Despite using a simple feature representation, the model is able to classify multiple hand gestures with reasonable performance, highlighting the potential of gesture recognition systems in real-world applications.

---

