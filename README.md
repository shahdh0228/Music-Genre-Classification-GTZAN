# 🎵 Music Genre Classification using GTZAN Dataset

## 📌 Project Overview
This project focuses on classifying music tracks into genres using machine learning and deep learning techniques. The GTZAN dataset was used to train models using both extracted audio features and spectrogram images.

The goal was to compare traditional machine learning models with deep learning approaches for multi-class music genre classification.


## 🎯 Problem Statement
Build a system that classifies songs into genres based on audio characteristics. The project explores two approaches:

1. **Tabular Approach** – Using extracted audio features such as MFCCs and spectral statistics.
2. **Image-Based Approach** – Using spectrogram images with CNN models.


## 📊 Dataset
Dataset used: **GTZAN Music Genre Dataset**

Kaggle Source:  
🔗 https://www.kaggle.com/code/imchentouf/gtzan-music-genre-classification/input

The dataset contains 10 music genres:

- Blues
- Classical
- Country
- Disco
- HipHop
- Jazz
- Metal
- Pop
- Reggae
- Rock

Two data formats were used:

1. **Extracted audio features**
   - MFCCs
   - Spectral centroid
   - Spectral bandwidth
   - Zero crossing rate
   - Chroma features

2. **Spectrogram images**
   - Generated visual representation of audio signals.


## 🛠 Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Librosa
- Matplotlib
- Seaborn


## 🔍 Methods Implemented

### 1️⃣ Tabular Feature-Based Models
Using extracted audio features:

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest

Features were scaled and used for multi-class classification.


### 2️⃣ CNN on Spectrogram Images
A Convolutional Neural Network (CNN) was trained using spectrogram images of songs to classify genres.

CNN architecture included:
- Convolution layers
- MaxPooling layers
- Dense layers
- Dropout for regularization


### 3️⃣ Transfer Learning (Bonus)
Transfer learning was implemented using **MobileNetV2** pretrained on ImageNet to improve spectrogram classification performance.


## 📈 Results

| Approach | Accuracy |
|--------|--------|
| Tabular (Best Model) | **80%** |
| CNN | **63%** |
| Transfer Learning | **59%** |

### Key Insight
Traditional machine learning using extracted audio features outperformed deep learning models trained on spectrogram images due to the relatively small dataset size.
