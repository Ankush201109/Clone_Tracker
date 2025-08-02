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

 ##Visual Effects Engine

**🎨 Color Gradient System
HSV to RGB conversion

Smooth gradient cycling

Pulsing via sine wave modulation

**💡 Neon Glow Effects
Dual-layer line drawing for glow

Joint circles with bright centers

Layer blending with cv2.addWeighted

**🌀 Motion Trails
Stores 8-frame trail history

Fades older trails with alpha blending

##3D Visualization
Real-time 3D plot of skeleton

Line + scatter points for connections

Same color scheme as 2D view

**🔧 Utility Functions
get_gradient_color(t) → Time-based color generator

draw_smooth_line() → Neon glowing lines

draw_smooth_circle() → Smooth joint highlights

**🔁 Main Loop
Read and flip webcam frame

Run pose detection

Apply visual effects

Update 3D skeleton every 6 frames

Show result in OpenCV + Matplotlib windows
