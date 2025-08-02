# Clone_Tracker

# 🧍‍♂️ Clone Tracker - Real-Time Pose Mirroring System

A visually stunning, real-time pose tracking application that mirrors your body movement into a glowing "clone" with 2D and 3D visualizations using MediaPipe and OpenCV.

---

## 🎯 Overview

**Clone Tracker** is an interactive system that:
- Detects full-body poses in real-time
- Creates a mirrored "clone" with pulsing neon glow
- Displays a synchronized 3D skeletal model
- Uses dynamic color gradients and smooth motion trails

Perfect for experiments in human motion visualization, AR/VR prototyping, educational demos, or interactive installations.

---

## ✨ Features

- ✅ **Real-Time Pose Detection**  
  Powered by [MediaPipe Pose](https://google.github.io/mediapipe/solutions/pose) (33 landmarks per person)

- 🪞 **Clone/Mirror Effect**  
  Creates a horizontally flipped version of your pose

- 🌈 **Dynamic Visual Effects**
  - Color-changing neon skeletal overlay
  - Pulsing glow using sine wave intensity
  - Joint trails that fade out over time
  - Time-based gradient transitions

- 🧠 **Dual Visualization**
  - 2D camera feed with visual effects
  - 3D real-time skeleton in a separate plot window

- ⚙️ **Performance Optimized**
  - FPS monitoring
  - Selective 3D updates for smoother performance
  - Efficient rendering with OpenCV

---

## 📦 Requirements

Install the following Python dependencies:

```bash
pip install opencv-python mediapipe numpy matplotlib
