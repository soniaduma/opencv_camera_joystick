# 🎮 Vision-Based Mouse Controller (OpenCV)

A real-time computer vision project that transforms a colored object into a virtual joystick for mouse control using a webcam.

This project demonstrates practical applications of image processing, contour detection, geometric analysis, and system interaction through automation.

---

## Overview

The application detects a predefined color in a live webcam feed and converts its position into directional mouse movement.

The movement speed is dynamically adjusted based on distance from the screen center using configurable sensitivity zones.

---

## Architecture

1. Capture webcam frame
2. Apply color mask
3. Detect contours
4. Select largest contour
5. Compute centroid
6. Calculate:
   - Distance from center
   - Angle of movement
7. Map angle to directional vector
8. Move mouse with dynamic sensitivity

---

## Technologies

- Python 3
- OpenCV
- NumPy
- PyAutoGUI

---

## Installation

```bash
git clone https://github.com/soniaduma/opencv_camera_joystick
cd opencv_camera_joystick
python -m venv venv
source venv/Scripts/activate   # Windows (Git Bash)
pip install -r requirements.txt
```

Made by a human for humans, please hire me: soniaduma.dev