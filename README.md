# DL-Project_Athlete-Fatigue-Prediction
# 🧠 Athlete Fatigue Prediction using Deep Learning

This project presents a Deep Learning approach to classify **athlete fatigue levels** using **sensor-based data** (accelerometer and gyroscope readings) from the [UCI Human Activity Recognition Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones).


## 📊 Dataset

- **Source**: UCI Human Activity Recognition (HAR) dataset
- **Sensor Data**: Accelerometer & Gyroscope
- **Subjects**: 30 participants performing activities like treadmill running, stair climbing, and resting.
- **Features**: 562 sensor measurements
- **Target Classes**:
  - `0` – Rest
  - `1` – Low Fatigue (Stair Descending)
  - `2` – Moderate Fatigue (Stair Ascending)
  - `3` – High Fatigue (Treadmill)

---

## 🧠 Model Overview

A **Dense Neural Network (Feedforward)** was used for multiclass classification of fatigue levels.

### Architecture:
- **Input Layer**: 562 features
- **Hidden Layers**: 
  - 256 neurons + ReLU
  - Dropout (50%)
  - 128 neurons + ReLU
  - Dropout (50%)
- **Output Layer**: 4 neurons + Softmax

### Compilation:
- **Loss Function**: Sparse Categorical Crossentropy
- **Optimizer**: Adam
- **Metric**: Accuracy

---

## 🛠 Implementation Highlights

- **Preprocessing**: Standard scaling of features, strategic activity relabeling
- **Regularization**: Dropout layers to prevent overfitting
- **Evaluation**: Confusion matrix, accuracy/loss trends over epochs
- **Validation**: Cross-validation ensures reliability across data splits

---

## 🧩 Future Scope

- Integration with **wearable devices** for real-time fatigue tracking
- Extendable to other athletic activities and sports
- Scope for **LSTM**/sequence-based models to capture temporal dependencies

---
