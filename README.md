

# Intelligent Sign Language Communication and Emergency Detection System using Computer Vision and Machine Learning

## Project Overview

The **Intelligent Sign Language Communication and Emergency Detection System using Computer Vision and Machine Learning** is designed to improve communication and safety for deaf and mute individuals. The system performs real-time sign language recognition using computer vision techniques and incorporates an emergency alert mechanism to detect predefined emergency gestures.

The system utilizes **MediaPipe** to detect and track hand landmarks from live video input. The extracted hand keypoints are converted into numerical feature representations and processed using both Machine Learning and Deep Learning models. K-Nearest Neighbors (KNN) is used as the baseline classifier, while Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks improve gesture recognition by learning spatial and temporal features.

The recognized gestures are converted into meaningful text using a time-based sentence formation mechanism. In addition, the system detects predefined emergency gestures such as **Help**, **Danger**, and **Emergency**, triggering an alarm and sending WhatsApp notifications along with location details using PyWhatKit. 

---

# Features

## Real-Time Gesture Recognition

* Real-time hand gesture recognition
* Webcam-based video input
* Hand landmark detection using MediaPipe
* Gesture-to-text conversion
* Sentence formation using sequential logic

## Machine Learning & Deep Learning

* K-Nearest Neighbors (KNN)
* Convolutional Neural Network (CNN)
* Long Short-Term Memory (LSTM)
* Feature extraction using hand landmarks

## Emergency Detection

* Detects predefined emergency gestures
* Alarm activation
* WhatsApp message generation
* Location sharing using PyWhatKit

---

# System Architecture

```text
                    Camera Input
                         │
                         ▼
              MediaPipe Hand Detection
                         │
                         ▼
              Hand Landmark Extraction
                         │
                         ▼
               Feature Representation
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
        KNN            CNN            LSTM
          │              │              │
          └──────────────┼──────────────┘
                         ▼
               Gesture Recognition
                         │
           ┌─────────────┴─────────────┐
           ▼                           ▼
    Sentence Formation         Emergency Detection
           │                           │
           ▼                           ▼
     Text Generation        Alarm + WhatsApp Alert
```

---

# Application Workflow

```text
Start
  │
  ▼
Capture Live Video
  │
  ▼
Detect Hand
  │
  ▼
Extract Hand Landmarks
  │
  ▼
Generate Feature Vectors
  │
  ▼
KNN Classification
  │
  ▼
CNN Feature Learning
  │
  ▼
LSTM Sequence Learning
  │
  ▼
Gesture Recognition
  │
  ▼
Sentence Formation
  │
  ▼
Check Emergency Gesture
  │
  ├──────────────No──────────────► Display Text
  │
 Yes
  │
  ▼
Activate Alarm
  │
  ▼
Send WhatsApp Message
  │
  ▼
Share Location
```

---

# Objectives

* Design and implement a real-time sign language recognition system using computer vision.
* Detect hand gestures and convert them into readable text.
* Develop a text-to-sign conversion module.
* Utilize Machine Learning and Deep Learning models such as KNN, CNN, and LSTM.
* Implement sentence formation using time-based sequential logic.
* Detect predefined emergency gestures.
* Trigger alerts including alarm activation and location-based messaging.
* Develop a user-friendly system suitable for real-world applications. 

---

# Tools and Technologies

| Category             | Technologies      |
| -------------------- | ----------------- |
| Programming Language | Python            |
| Computer Vision      | OpenCV, MediaPipe |
| Machine Learning     | KNN               |
| Deep Learning        | CNN, LSTM         |
| Data Processing      | NumPy, Pandas     |
| Automation           | PyWhatKit         |
| Alarm                | Pygame            |



---

# Project Structure

```text
Intelligent-Sign-Language-Communication-System/
│
├── dataset/
├── models/
├── notebooks/
├── output/
├── README.md
├── requirements.txt
└── main.py
```

> **Note:** Your report does **not** include a project directory structure. The above is only a placeholder structure for organizing the repository.

---

# Methodology

1. Capture live video through a webcam.
2. Detect hand landmarks using MediaPipe.
3. Convert landmarks into numerical feature vectors.
4. Perform gesture classification using KNN.
5. Extract spatial features using CNN.
6. Capture temporal dependencies using LSTM.
7. Convert recognized gestures into meaningful sentences.
8. Monitor for emergency gestures.
9. Trigger alarms and send WhatsApp messages with location details when emergencies are detected. 

---

# Future Scope

* Support larger gesture datasets.
* Multiple language support.
* Mobile deployment.
* Integration with advanced AI models.
* Improved scalability and real-world applications. 

---

# Project Status

Status:Major Academic Project(In progress)
Completion:Approximately 70% complete
Developed as a Major Academic Project for the Bachelor of Engineering (B.E.) in Computer Science & Engineering, with core functionalities completed and testing and optimization currently in progress.



---

This version stays faithful to your report. The only section that is **not** from the report is the **Project Structure**, because your report does not describe the repository layout. Everything else is derived directly from the report.
