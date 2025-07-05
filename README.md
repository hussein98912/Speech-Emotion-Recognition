# 🎙️ Speech Emotion Recognition from Audio

A deep learning-based system to recognize emotions from speech using the [RAVDESS](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio) dataset. This project extracts audio features (MFCCs) and classifies emotional states using LSTM/CNN architectures.

---

## 📌 Overview

This project aims to classify spoken audio clips into the following emotions:

- 😐 Neutral  
- 😌 Calm  
- 😄 Happy  
- 😢 Sad  
- 😠 Angry  
- 😨 Fearful  
- 🤢 Disgust  
- 😲 Surprised  

It achieves high classification accuracy using MFCC (Mel Frequency Cepstral Coefficients) features and a deep learning model trained on the RAVDESS dataset.
---

## 📌 Project Highlights

- 📁 Loaded & preprocessed over **1,400 WAV** files.
- 🧠 Applied **MFCC extraction** (Mel-frequency cepstral coefficients).
- 🧪 Performed **data augmentation**: noise addition, pitch shifting, time stretching, and shifting.
- 🧮 Built a deep neural network using **TensorFlow/Keras**.
- 🎯 Achieved an accuracy of **~87%** on test data.
- 📊 Visualized class distribution and training metrics.

---

## 🔧 Data Preprocessing

- Extracted 40 MFCCs per frame
- Zero-padded all features to a max length of 174
- Encoded emotions using `LabelEncoder`
- Balanced the dataset by selectively sampling classes

---

## 🗃️ Dataset

- **Name**: RAVDESS Emotional Speech Audio
- **Size**: 24 professional actors (12 male, 12 female)
- **Classes**: Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised (we selected a subset)
- 📥 [Download Dataset from Kaggle](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio)

---

## 🛠️ Features

- 🎧 Audio signal processing with `librosa`
- 🔊 Feature extraction using MFCCs
- 📊 Training deep neural networks (LSTM / CNN)
- 📈 Visualization of training and evaluation
- 🧪 Early stopping & validation monitoring

---

## 📊 Results

- **Train/Test Split:** 80% training, 20% testing  
- **Epochs:** 50 (with EarlyStopping)  
- **Batch Size:** 32  
- **Final Test Accuracy:** **87%**

### 🧾 Classification Report

| Emotion    | Precision | Recall | F1-Score |
|------------|-----------|--------|----------|
| Happy      | 0.92      | 0.91   | 0.92     |
| Sad        | 0.85      | 0.89   | 0.87     |
| Angry      | 0.82      | 0.80   | 0.81     |
| Calm       | 0.85      | 0.86   | 0.85     |
| Neutral    | 0.92      | 0.92   | 0.92     |
| Fearful    | 0.83      | 0.82   | 0.82     |
| Disgust    | 0.88      | 0.86   | 0.87     |
| Surprised  | 0.89      | 0.88   | 0.88     |

> 📌 **Observation:** The model shows strong performance across all emotions.

---
