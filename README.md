# 👁️ Eye Gaze Tracking System

An AI-powered mobile-based eye gaze tracking system that predicts where the user is looking on the screen using only the front camera.

The project uses facial landmark detection and gaze-region prediction to enable real-time gaze estimation for human-computer interaction applications.

---

# 📸 Screenshots

## 🏠 Application Home Screen

<p align="center">
  <img width="796" height="1560" alt="image" src="https://github.com/user-attachments/assets/50eaf216-bffc-4312-abc3-d151bb0ad21d" />

</p>

---

## 👀 Gaze Tracking Interface

<p align="center">
  <img width="512" height="1036" alt="image" src="https://github.com/user-attachments/assets/786681d1-4a09-433a-867e-17c7d8574d86" />


</p>

---

# ✨ Features

✅ Real-time eye gaze tracking  
✅ Mobile camera-based inference  
✅ Facial and eye landmark extraction  
✅ 9×9 grid-based gaze prediction  
✅ Lightweight and efficient pipeline  
✅ Flask backend for processing  
✅ React Native frontend integration  
✅ Dataset collection mode  
✅ Testing and video-based inference modes  

---

# 🛠️ Tech Stack

## 📱 Frontend
- React Native
- Expo Go

## ⚙️ Backend
- Flask
- Python

## 🤖 AI / Computer Vision
- MediaPipe Face Mesh
- OpenCV
- NumPy

---

# 🏗️ Project Architecture

The system consists of three major components:

1️⃣ Mobile Application  
2️⃣ Backend Processing Server  
3️⃣ Gaze Prediction Pipeline  

---

# 🔄 Workflow

## 1️⃣ Data Collection

The mobile screen is divided into a **9×9 grid** representing different gaze regions.

The user looks at predefined grid positions while the front camera captures video frames.

The collected data is used for supervised gaze prediction.

---

## 2️⃣ Landmark Detection

MediaPipe Face Mesh is used to extract facial and eye landmarks from each frame.

The system focuses on:
- 👁️ Eye corner points
- 🎯 Iris positions
- 📐 Eye geometry

---

## 3️⃣ Feature Extraction

Instead of using raw images directly, landmark coordinates are used as structured numerical features.

This reduces:
- ⚡ Computational complexity
- 🔇 Noise
- 📉 Training requirements

while improving real-time performance.

---

## 4️⃣ Gaze Prediction

The extracted landmark features are mapped to corresponding screen regions.

The system predicts one of the **81 possible gaze regions** on the screen.

---

# 🧠 AI Concepts Used

- Computer Vision
- Facial Landmark Detection
- Eye Tracking
- Supervised Learning
- Real-Time Inference
- Grid-based Classification
- Feature Engineering

---

# 🚀 Why MediaPipe?

MediaPipe provides:

✅ Lightweight real-time inference  
✅ Robust facial landmark detection  
✅ Mobile-friendly performance  
✅ Efficient eye tracking capabilities  

making it suitable for real-time gaze estimation systems.

---

# ⚠️ Challenges Faced

- 💡 Lighting variations
- 🧍 Head movement
- 👤 Different user face structures
- 📷 Camera angle inconsistencies
- ⚡ Real-time processing constraints

---

# 🔮 Future Improvements

- Personalized calibration
- Continuous coordinate prediction
- Transformer-based gaze estimation
- Improved iris tracking
- On-device AI inference
- Accessibility-focused interaction systems

---

# 🌍 Applications

✅ Accessibility systems  
✅ Hands-free interaction  
✅ Gaze-controlled keyboards  
✅ Human-computer interaction  
✅ Assistive technologies  
✅ Smart interfaces  

---

# ⚙️ Installation

## 📥 Clone Repository

```bash
git clone https://github.com/Manan1801/eye-model.git
cd eye-model
```

## 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

## ▶️ Run Backend

```bash
python app.py
```

---

# 📁 Project Structure

```plaintext
eye-model/
│
├── backend/
├── frontend/
├── models/
├── utils/
├── dataset/
├── screenshots/
├── app.py
├── requirements.txt
└── README.md
```

---

# 👨‍💻 Authors

- Manan Chavda
- Lakshya Kesarwani

---

# 📚 References

- MediaPipe Face Mesh
- OpenCV Documentation
- Real-Time Gaze Estimation Research Papers

---

# 📜 License

This project is developed for educational and research purposes.
