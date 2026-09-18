# Computer Vision Based Automated Face Attendance System

## Overview
A real-time Computer Vision system designed in Python and OpenCV. It captures frames from live webcam devices, isolates face regions using multi-scale object detection classifiers, and updates student attendance records into a structured CSV file automatically.

## Features
- Real-time webcam processing pipeline.
- Facial region detection using OpenCV Haar Cascade Classifiers.
- Automatic attendance log generation (`attendance.csv`).
- Built-in duplicate entry protection per calendar date.

## Technologies Used
- **Language:** Python 3.x
- **Computer Vision Framework:** OpenCV (`cv2`)
- **Data & System Utilities:** NumPy, Datetime, CSV, OS

## Installation & Setup
1. Clone repository:
   ```bash
   git clone [https://github.com/devpatelgeek/Smart-Face-Attendance-CV.git](https://github.com/devpatelgeek/Smart-Face-Attendance-CV.git)
   cd Smart-Face-Attendance-CV