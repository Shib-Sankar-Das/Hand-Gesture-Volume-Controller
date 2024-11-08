# 🎛️ Hand Gesture Volume Controller

Welcome to the **Hand Gesture Volume Controller** project! This project leverages computer vision and hand-tracking technology to control your device's volume simply by using hand gestures. Say goodbye to reaching for volume buttons – now, just pinch or move your fingers to adjust the volume effortlessly! 🎶

---

## 📋 Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Project Approach](#project-approach)
- [How to Run](#how-to-run)
- [Libraries Used](#libraries-used)
- [Screenshots](#screenshots)
- [License](#license)

---

## 🖥️ Introduction
This project uses **OpenCV** and **MediaPipe** to track hand movements in real-time through your webcam, and **PyCaw** to interact with the system's audio. It uses a simple yet effective method to recognize hand gestures, specifically the pinch motion, to increase or decrease the volume. Designed to be intuitive and smooth, the program runs in the background without needing any physical interaction with your device’s audio controls.

---

## ✨ Features
- **Real-Time Hand Tracking** – Detects hands and fingers in real-time using a webcam.
- **Gesture-Based Volume Control** – Adjust the volume by moving your fingers closer or apart.
- **Visual Feedback** – Displays visual cues on the screen for an enhanced user experience.
- **Dynamic Range Control** – Automatically maps hand movement range to volume control range.
- **Smooth Operation** – Gesture smoothing for a more stable volume adjustment.

---

## 🔍 Project Approach
The project combines **MediaPipe's hand-tracking capabilities** with **PyCaw's audio control**. Here’s how it works:

1. **Hand Detection**: MediaPipe locates and tracks hands, recognizing key landmarks.
2. **Gesture Recognition**: Specific landmarks on fingers (such as the thumb and index finger) are monitored to detect gestures.
3. **Distance Calculation**: Using Euclidean distance between landmarks, the pinch gesture is recognized and translated into volume control commands.
4. **Volume Adjustment**: Based on the distance between landmarks, the system maps the gesture range to the device's volume range and sets the volume level accordingly.
5. **Real-Time Display**: Provides real-time feedback on screen, showing the volume level, percentage, and current FPS.

---

## ⚙️ How to Run
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/Shib-Sankar-Das/Hand-Gesture-Volume-Controller.git
    ```

2. **Install Required Libraries**:
    Ensure you have Python 3.x installed, then install dependencies:
    ```bash
    pip install opencv-python mediapipe pycaw numpy comtypes
    ```

3. **Run the Script**:
    ```bash
    python HandGestureVolumeControl.py
    ```
    *Note: Ensure your system has a working webcam.*

4. **Adjust Volume with Your Hand**:
   - Use your thumb and index finger in a pinch gesture.
   - Moving fingers closer or farther apart will decrease or increase the volume, respectively.

---

## 📚 Libraries Used
- **OpenCV** – For video capture and image processing.
- **MediaPipe** – For hand tracking and gesture recognition.
- **PyCaw** – To interact with the system's audio control.
- **Numpy** – For mathematical operations.
- **Comtypes** – For working with Windows COM objects (required by PyCaw).

---

## 📸 Screenshots
Here are some example screenshots of the Hand Gesture Volume Controller in action!

![Screenshot 2024-11-08 155431](https://github.com/user-attachments/assets/b1bcfb7a-57a7-47d7-becd-e0a3f601c1d7)


