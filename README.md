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

## 🧠 Model Summary

- **Preprocessing**: MFCC extraction using Librosa
- **Model Architectures**: CNN and LSTM-based deep learning models
- **Accuracy Achieved**: **~88%**
- **Framework**: TensorFlow / Keras

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

| Emotion | Precision | Recall | F1-Score |
|---------|-----------|--------|----------|
| Neutral | 0.92      | 0.92   | 0.92     |
| Calm    | 0.85      | 0.86   | 0.85     |
| Happy   | 0.92      | 0.91   | 0.92     |
| Sad     | 0.85      | 0.89   | 0.87     |
| Angry   | 0.82      | 0.80   | 0.81     |

- ✅ Overall Accuracy: **88%**

### 📈 Accuracy & Loss Curves
![Accuracy Plot](images/accuracy_plot.png)

### 📉 Confusion Matrix
![Confusion Matrix](images/confusion_matrix.png)

---
