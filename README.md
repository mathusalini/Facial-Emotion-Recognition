# Facial-Emotion-Recognition# 😊 Facial Emotion Recognition (Google Colab Version)

## 📌 Project Overview

This project demonstrates **Facial Emotion Recognition using a live webcam feed inside Google Colab**.

Since Google Colab runs on a remote server and does not allow direct webcam access using `cv2.VideoCapture(0)`, this project uses:

- 🔹 JavaScript (Browser Webcam Access)
- 🔹 Python + OpenCV
- 🔹 PyTorch-based Emotion Recognition Model
- 🔹 Google Colab Integration

The system captures webcam images from the browser and performs emotion detection on each captured frame.

---

## 🎯 Objective

To detect human facial emotions such as:

- 😀 Happy  
- 😢 Sad  
- 😠 Angry  
- 😲 Surprise  
- 😐 Neutral  
- 😨 Fear  
- 🤢 Disgust  

using a deep learning model in a cloud-based environment.

---

## ⚙️ How It Works

### 1️⃣ Webcam Access (Browser Side)

Google Colab cannot directly access your webcam.

So we:

- Use JavaScript (`navigator.mediaDevices.getUserMedia`)
- Capture image frame in browser
- Convert image to Base64 format
- Send image to Python backend

---

### 2️⃣ Emotion Detection (Python Side)

- Image decoded using OpenCV
- Frame passed into `EmotionRecognition`
- Model predicts emotion
- Emotion label drawn on detected face
- Processed image displayed in Colab output

---
## 🎓 Learning Outcomes

After completing this project, you will understand:

- Browser-to-Python communication  
- Webcam handling in cloud environments  
- PyTorch model loading on CPU  
- Deep learning inference pipeline  
- Real-time computer vision workflow  

---

## 💡 Future Improvements

- Convert into a Streamlit Web Application  
- Add live video streaming support  
- Deploy on a cloud server  
- Use GPU acceleration  
- Add emotion confidence score visualization  
