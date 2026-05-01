# Real-Time Emotion Recognition using DeepFace & OpenCV

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/OpenCV-Computer_Vision-green?style=for-the-badge&logo=opencv">
  <img src="https://img.shields.io/badge/DeepFace-AI-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
</p>

---

## Overview

This project implements a **real-time facial emotion recognition system** using **DeepFace** and **OpenCV**.
It captures webcam input, detects faces, and classifies emotions instantly.

Recognized emotions:

* 😊 Happy
* 😢 Sad
* 😡 Angry
* 😮 Surprise
* 😐 Neutral
* 😨 Fear
* 🤢 Disgust

---

## Objectives

* Real-time face detection
* Emotion classification using AI
* Live visualization using bounding boxes
* Lightweight and easy-to-run implementation

---

## Tech Stack

* Python
* OpenCV
* DeepFace
* Haar Cascade Classifier

---

## Project Structure

```
Emotion-Recognition-Using-DeepFace-and-OpenCV/
│── emotion.py   ← main file
│── requirements.txt
│── README.md
│── haarcascade_frontalface_default.xml
│── assets/
│     └── demo.png
```

---

# Setup Guide

## 1. Clone Repository

```bash
git clone https://github.com/mahnoorabrar/Emotion-Recognition-Using-DeepFace-and-OpenCV.git
cd Emotion-Recognition-Using-DeepFace-and-OpenCV
```

---

## 2. Create Virtual Environment (Recommended)

```bash
python -m venv venv
```

### Activate:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / Mac**

```bash
source venv/bin/activate
```

---

## 3. Install Requirements

```bash
pip install -r requirements.txt
```

---

## 4. Download Haar Cascade File

* Visit: https://github.com/opencv/opencv/tree/master/data/haarcascades
* Download: `haarcascade_frontalface_default.xml`
* Place it in project folder

---

## 5. Run the Project

```bash
python emotion.py
```

🎥 Webcam will open
😊 Faces will be detected
🧠 Emotions will appear on screen

Press **'q'** to exit.

---

# How It Works

### Pipeline

```
Webcam → Face Detection → ROI → DeepFace → Emotion → Display
```

---

## Steps

1. Capture webcam frames
2. Convert frame to grayscale
3. Detect faces using Haar Cascade
4. Extract face region (ROI)
5. Convert to RGB
6. Analyze using DeepFace
7. Get dominant emotion
8. Draw bounding box and label
9. Display output

---


## Results

* Real-time detection
* Accurate predictions
* Fast performance (hardware dependent)

---

## Limitations

* Sensitive to lighting
* Performance drops on low-end systems
* Occlusion affects accuracy

---

## Future Improvements

* Add age & gender detection
* Deploy on Jetson Nano
* Improve FPS
* Add tracking system

---

## Troubleshooting

### Camera not opening

* Close other apps using camera

### Module error

```bash
pip install deepface opencv-python
```

### Slow performance

* Close background apps
* Use GPU if available

---

## 👩‍💻 Author

**Mahnoor Abrar**
🔗 https://github.com/mahnoorabrar

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
