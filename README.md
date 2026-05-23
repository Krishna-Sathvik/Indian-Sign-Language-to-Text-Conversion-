# Sign Language to Text Conversion

## Overview

This project focuses on real-time Indian Sign Language (ISL) recognition and conversion into readable text using Deep Learning and Computer Vision techniques. The system captures hand gestures through a webcam, extracts hand landmarks using MediaPipe, and classifies gestures using a Convolutional Neural Network (CNN) trained on a large gesture dataset.

The project aims to improve accessibility and communication support for hearing-impaired individuals through real-time gesture-to-text translation.

---

## Project Objective

The primary objective of this project is to develop an AI-powered sign language recognition system capable of:

* Detecting hand gestures in real time
* Extracting meaningful hand landmarks
* Classifying Indian Sign Language gestures accurately
* Converting gestures into readable text instantly
* Providing an accessible communication interface for hearing-impaired users

---

## Problem Statement

Communication barriers faced by hearing-impaired individuals often require sign language interpreters, which may not always be available.

Traditional gesture recognition systems struggle with:

* Real-time processing
* Accurate hand tracking
* Environmental variations
* Complex gesture patterns

This project addresses these challenges by combining:

* MediaPipe hand landmark detection
* CNN-based gesture classification
* Real-time OpenCV video processing

to create an efficient gesture-to-text conversion system.

---

## Technologies Used

| Category             | Technologies                       |
| -------------------- | ---------------------------------- |
| Programming Language | Python                             |
| Deep Learning        | TensorFlow, Keras                  |
| Computer Vision      | OpenCV                             |
| Hand Tracking        | MediaPipe                          |
| Data Processing      | NumPy, Pandas                      |
| Visualization        | Matplotlib                         |
| Model Type           | Convolutional Neural Network (CNN) |

---

## Dataset Information

### Dataset Details

* Dataset Type: Indian Sign Language Gesture Images
* Total Images: 15,000+
* Classes: Multiple ISL Alphabets/Gestures
* Image Format: Grayscale/RGB Gesture Images

### Data Preprocessing

The preprocessing pipeline includes:

* Image resizing
* Normalization
* Landmark extraction
* Data augmentation
* Train-test split generation

---

## Project Workflow

### 1. Real-Time Video Capture

OpenCV is used to capture live webcam video frames for gesture detection.

### 2. Hand Detection using MediaPipe

MediaPipe extracts:

* Hand landmarks
* Finger joint positions
* Hand coordinates

This significantly improves gesture tracking efficiency.

### 3. Data Preprocessing

Captured hand regions are:

* Cropped
* Resized
* Normalized
* Converted into CNN-compatible format

### 4. CNN Model Training

The CNN model learns gesture patterns from the ISL dataset.

### 5. Real-Time Gesture Classification

The trained model predicts gesture labels in real time.

### 6. Gesture-to-Text Conversion

Predicted gestures are converted into readable text output.

---

## CNN Architecture

y = f(Wx + b)

The project uses a Convolutional Neural Network (CNN) to classify sign language gestures based on extracted hand features and image patterns.

The CNN helps:

* Detect gesture shapes
* Learn spatial image patterns
* Improve classification accuracy

---

## Model Performance

| Metric                  | Value          |
| ----------------------- | -------------- |
| Classification Accuracy | 95%            |
| Dataset Size            | 15,000+ Images |
| Detection Speed         | 30 FPS         |
| Processing Type         | Real-Time      |

The system achieved high real-time recognition accuracy while maintaining smooth video processing performance.

---

## Notebook Outputs

### CNN Training Accuracy
<img width="536" height="352" alt="isl training accuracy" src="https://github.com/user-attachments/assets/561fad68-5f00-4ce2-aa8d-8bacf41fd587" />

### Training Loss Curve
<img width="535" height="352" alt="isl training loss" src="https://github.com/user-attachments/assets/2267ded7-2cde-4c1e-ae65-2005ddabc9b5" />

### Confusion Matrix
<img width="346" height="249" alt="image" src="https://github.com/user-attachments/assets/84061856-6c1a-49c4-8d8a-027ee831c1e1" />


### Real-Time Gesture Detection
<img width="834" height="67" alt="image" src="https://github.com/user-attachments/assets/1f536aa2-8645-4e71-a234-2ae24dfd00ae" />


### Real-Time Prediction

The system displays:

* Detected gesture
* Converted text output
* Live webcam feed

Example output:

```python
Predicted Gesture: HELLO
Converted Text: HELLO
```

---

## Key Features

* Real-time sign language detection
* CNN-based gesture classification
* MediaPipe hand landmark extraction
* OpenCV webcam integration
* Fast inference with 30 FPS performance
* Gesture-to-text translation
* Accessibility-focused application

---

## Key Learning Outcomes

This project helped implement and understand:

* Computer Vision fundamentals
* CNN-based image classification
* Real-time AI inference pipelines
* Hand landmark detection
* Deep Learning model training
* Gesture recognition systems
* Human-computer interaction concepts

---

## Required Libraries

```
python
tensorflow
keras
opencv-python
mediapipe
numpy
pandas
matplotlib
```

---

### Real-Time Detection

* Open webcam
* Show sign gesture
* System predicts gesture
* Gesture converts into text

---

## Future Improvements

Potential future enhancements include:

* Sentence-level sign recognition
* Transformer-based gesture models
* Multi-hand gesture support
* Voice output generation
* Mobile application deployment
* Real-time sentence correction
* Support for multiple sign languages

---

## Conclusion

This project demonstrates the practical implementation of deep learning and computer vision techniques for accessibility-focused applications. By combining CNN-based gesture classification with MediaPipe hand tracking and OpenCV video processing, the system successfully performs real-time sign language recognition and gesture-to-text conversion with high accuracy and efficient performance.

---

## Author

**Cheedu Krishna Sathvik Reddy**

* B.Tech CSE (AI & ML)
* VNR Vignana Jyothi Institute of Engineering and Technology
* Hyderabad, India
