# ✋ Gesture Recognition

## 📘 Overview
This module focuses on recognizing **hand gestures** using computer vision and deep learning techniques.  
The goal is to detect and classify human hand gestures in real-time or from image/video data.

---

## 🎯 Objective
- Build a model to **recognize different hand gestures** from image or video input.  
- Use **landmark detection** and **machine learning** for classification.  
- Demonstrate **feature extraction**, **model training**, and **inference** steps.

---

## 🧩 Approach

### 1️⃣ Dataset
- **Source:** [Hand Gesture Dataset](https://drive.google.com/drive/folders/1F35-FyjwFcTQD_dg3qkz16WWGgYMGJWN?usp=drive_link)
- Contains multiple labeled gesture images.
- Data split into **train**, **validation**, and **test** sets.
- I have taken **5 photos from each gesture class** in the dataset to analyse algorithm.

### 2️⃣ Preprocessing
- Image resizing and normalization  
- Hand landmark detection using **MediaPipe Hands**  
- Conversion of landmarks into numerical feature vectors  
- Label encoding for gesture categories

### 3️⃣ Model Architecture
- Implemented a **CNN** (or optionally CNN+LSTM) based model for gesture classification  
- Key layers:
  - Convolutional layers (feature extraction)
  - Flatten + Dense layers (classification)
  - Softmax output for gesture labels

### 4️⃣ Training
- Optimizer: `Adam`
- Loss Function: `categorical_crossentropy`
- Metrics: `accuracy`
- Batch size and epochs tuned experimentally for best validation accuracy

### 5️⃣ Evaluation
- Tested the model using **5 sample images from each gesture class** to check real-world prediction reliability.
- Accuracy and confusion matrix used to assess performance  
- Visualized predictions using sample test images  
- Exported trained model for inference

---

## 📂 Folder Structure
