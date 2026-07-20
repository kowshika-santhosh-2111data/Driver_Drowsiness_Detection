# Driver Drowsiness Detection using Eye Closure and Yawning Analysis with Deep Learning

## Project Overview

Driver drowsiness is one of the leading causes of road accidents worldwide. This project develops an intelligent real-time driver monitoring system that detects signs of fatigue by analyzing **eye closure** and **yawning** using Deep Learning.

The system classifies facial images into four categories:

* 👁️ Open Eyes
* 😴 Closed Eyes
* 🥱 Yawning
* 😊 No Yawn

Based on these predictions, the system determines the driver's alertness level and can be extended to trigger an alarm when drowsiness is detected.

---

## Objectives

* Detect driver drowsiness using facial features.
* Compare the performance of a Custom CNN and MobileNetV2.
* Improve detection accuracy using Transfer Learning.
* Build a reliable fatigue detection model suitable for real-time applications.

---

## Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab

---

## Dataset Structure

```text
Datas/
│── Open/
│── Closed/
│── yawn/
│── no_yawn/
```

The dataset contains images representing different driver facial states.

---

## Project Workflow

```
Dataset Collection
        ↓
Data Preprocessing
        ↓
Data Augmentation
        ↓
Train-Test Split
        ↓
Custom CNN Model
        ↓
MobileNetV2 Model
        ↓
Model Training
        ↓
Performance Evaluation
        ↓
Confusion Matrix
        ↓
Classification Report
        ↓
Single Image Prediction
        ↓
Driver Fatigue Analysis
```

---

## Data Preprocessing

* Loaded images from four classes
* Image resizing
* Image normalization
* Label encoding
* Train-Test Split
* Data Augmentation
* Saved processed NumPy arrays

---

## Models Implemented

### Custom CNN

* Convolution Layers
* Batch Normalization
* MaxPooling
* Global Average Pooling
* Dense Layers
* Dropout

### MobileNetV2 (Transfer Learning)

* Pre-trained MobileNetV2
* Feature Extraction
* Global Average Pooling
* Dense Layers
* Dropout
* Softmax Output Layer

---

## Performance Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

Performance graphs include:

* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss

---

## Features

* Image preprocessing
* Data augmentation
* Deep Learning model training
* Transfer Learning
* Single image prediction
* Driver fatigue analysis
* Performance visualization
* Model saving and loading

---

## Project Files

```
Data_Preprocessing.ipynb
CNN.ipynb
MobileNetV2.ipynb
mobilenet_driver_drowsiness.keras
cnn_driver_drowsiness.keras
README.md
```

---

## Future Enhancements

* Real-time webcam integration
* Face detection using MediaPipe or Dlib
* Eye Aspect Ratio (EAR) calculation
* Mouth Aspect Ratio (MAR) calculation
* Alarm notification system
* Low-light performance improvement
* Mobile application deployment
* Edge device implementation using TensorFlow Lite

---

## Results

The MobileNetV2 model achieved significantly better performance than the Custom CNN, demonstrating the effectiveness of transfer learning for driver drowsiness detection.

---

## Applications

* Smart Vehicles
* Driver Monitoring Systems
* Road Safety
* Fleet Management
* Transportation Industry
* Accident Prevention Systems

---
