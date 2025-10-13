# ✋ Gesture Recognition

## 📘 Overview
This project focuses on **gesture recognition** using the **MediaPipe Gesture Recognizer**.  
The goal was to detect and classify hand gestures from static images using a pre-trained `.task` model file, without training or evaluating a new model.

---

## 🎯 Objective
- Use **MediaPipe**’s gesture recognition model to identify gestures from images.  
- Perform **landmark detection** and **gesture classification** using pre-trained pipelines.  
- Visualize results with hand landmarks and gesture labels.

---

## 🧩 Approach

### 1️⃣ Dataset
- **Source:** [Hand Gesture Dataset](https://drive.google.com/drive/folders/1F35-FyjwFcTQD_dg3qkz16WWGgYMGJWN?usp=drive_link)
- I selected **5 photos from each gesture class** to **test the algorithm’s recognition ability**.
- These images were processed through the MediaPipe pipeline for gesture classification.

### 2️⃣ Pretrained Model
- Model used: `gesture_recognizer.task`
- Loaded via `mp.tasks.vision.GestureRecognizer`  
- This model predicts gesture type (e.g., “Thumbs Up”, “Victory”, “Open Palm”) directly from input images.

### 3️⃣ Implementation Details
- Framework: **MediaPipe** (Vision Tasks API)
- Libraries used:
  - `opencv-python`
  - `mediapipe`
  - `matplotlib`
  - `ipywidgets`
- The code:
  - Reads images from a folder.
  - Detects hands and landmarks.
  - Classifies the gesture using the pre-trained model.
  - Draws the hand landmarks and recognized gesture label on the image.
  - Saves annotated outputs for reference.

### 4️⃣ Evaluation
- This implementation is **not model training or evaluation** based.  
- No accuracy or performance metrics were calculated.  
- The focus was to **verify recognition capability** on small test samples (5 per class).

---
