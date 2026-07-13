# 👁️ DeepVision Attendance — Automated Face Recognition System

> **Published Research** — Global Conference on Information Technologies and Communications (GCITC) | September 2023

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer_Vision-green?logo=opencv)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep_Learning-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-CNN-red?logo=keras)
![Status](https://img.shields.io/badge/Status-Published-green)

---

## 📌 Overview

An advanced **automated attendance tracking system** using real-time face recognition. The system processes **multiple faces simultaneously** using a hybrid approach combining **Convolutional Neural Networks (CNN)** and **Histogram of Oriented Gradients (HOG)** for precise facial detection and identification.

Designed and evaluated on a dataset of **~1,000 students**, achieving a **40% improvement in operational efficiency** over manual attendance processes.

This work was presented and published at the **Global Conference on Information Technologies and Communications (GCITC), 2023**.

---

## 🎯 Key Results

| Metric | Result |
|--------|--------|
| Dataset Size | ~1,000 student records |
| Efficiency Improvement | **40%** over manual tracking |
| Detection Method | CNN + HOG hybrid |
| Processing | Multi-face simultaneous detection |
| Precision/Recall | Evaluated with false-positive analysis |
| Publication | GCITC 2023 |

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Deep Learning** | TensorFlow, Keras, CNN |
| **Computer Vision** | OpenCV, HOG (Histogram of Oriented Gradients) |
| **Language** | Python 3.8+ |
| **Face Detection** | dlib, face_recognition library |
| **Data Management** | Pandas, NumPy |
| **Model Evaluation** | Precision, Recall, F1, Confusion Matrix |
| **Environment** | Jupyter Notebook |

---

## 📊 What This Project Does

1. **Face Detection** — Real-time detection of multiple faces in a single frame using HOG
2. **Face Recognition** — CNN-based identification matching faces to student database
3. **Data Labelling** — Structured student image dataset with quality validation
4. **Attendance Marking** — Automatic attendance logging with timestamp
5. **False-Positive Analysis** — Statistical accuracy metrics to minimise misidentification
6. **Data Readiness** — Governed dataset with labelling quality checks for AI use case
7. **Reporting** — Automated attendance report generation per session

---

## 📁 Project Structure

```
deepvision-attendance-system/
│
├── data/
│   ├── student_images/               # Student face image dataset (~1000 records)
│   └── attendance_records/           # Generated attendance logs
│
├── models/
│   ├── cnn_face_recognition.h5       # Trained CNN model
│   └── hog_detector.pkl              # HOG face detector
│
├── notebooks/
│   ├── 01_data_preparation.ipynb     # Image collection + labelling pipeline
│   ├── 02_model_training.ipynb       # CNN training + validation
│   ├── 03_hog_detection.ipynb        # HOG detector implementation
│   ├── 04_evaluation.ipynb           # Precision, recall, false-positive analysis
│   └── 05_realtime_demo.ipynb        # Live face recognition demo
│
├── src/
│   ├── face_detector.py              # HOG + CNN detection pipeline
│   ├── attendance_tracker.py         # Attendance logging system
│   └── report_generator.py          # Attendance report output
│
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run

### Prerequisites
```bash
pip install tensorflow keras opencv-python dlib face_recognition pandas numpy
```

### Setup Dataset
```bash
# Add student images to data/student_images/
# Each student folder named: StudentID_Name/
# Minimum 5 images per student recommended
```

### Run the System
```bash
# Train the model
jupyter notebook notebooks/02_model_training.ipynb

# Run real-time attendance
python src/face_detector.py --camera 0

# Generate report
python src/report_generator.py --date 2024-01-15
```

---

## 📈 Model Performance

```
Evaluation Results (~1,000 students):
─────────────────────────────────────────────────────
Metric                  Score
─────────────────────────────────────────────────────
Detection Accuracy      94.2%
Precision               93.8%
Recall                  94.6%
F1-Score                94.2%
False Positive Rate     2.1%
Processing Speed        ~0.3 sec/face
─────────────────────────────────────────────────────
Efficiency vs Manual:   +40% improvement
```

---

## 🔍 How It Works

```
Camera Feed
    ↓
HOG Face Detector → Locates faces in frame
    ↓
CNN Face Recogniser → Matches face to student database
    ↓
Confidence Threshold → Filters false positives
    ↓
Attendance Logger → Marks present with timestamp
    ↓
Report Generator → Exports attendance CSV/PDF
```

---

## 🔬 Data Governance Applied

- **Data labelling quality checks** — every image validated before training
- **False-positive analysis** — statistical accuracy metrics prevent misidentification
- **Data readiness principles** — structured, labelled dataset ready for AI consumption
- **Privacy considerations** — local processing, no cloud upload of student images

---

## 📜 Publication

**Title:** DeepVision Attendance: A Visual Recognition System for Automated Attendance Tracking

**Conference:** Global Conference on Information Technologies and Communications (GCITC)

**Published:** September 2023

---

## 👤 Author

**Kona Mourya Sai Chandra**
- 📧 k.mourya77@gmail.com
- 💼 [LinkedIn](https://linkedin.com/in/Msc2003)
- 🐙 [GitHub](https://github.com/Mouryasai1)
