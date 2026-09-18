# 👁️ Smart Automated Face Attendance System (Computer Vision)

<div align="center">

![Python Version](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Computer Vision](https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Data Integrity](https://img.shields.io/badge/Database-CSV%20Persistence-228B22?style=for-the-badge)
![Academic Compliance](https://img.shields.io/badge/VITyarthi-Flipped%20Course%20Approved-FF6600?style=for-the-badge)

**An Enterprise-Grade Real-Time Biometric Attendance & Spatial Face Recognition Pipeline**

[Explore Code](#-project-structure) • [Installation](#-installation--quickstart-guide) • [Architecture](#-system-architecture--visual-pipeline) • [Author](#-academic-metadata--author-details)

</div>

---

## 🚀 Executive Project Summary

The **Smart Automated Face Attendance System** is a robust Computer Vision solution designed to automate physical attendance verification in academic and corporate environments. By replacing manual, paper-based roll calls with real-time digital image processing and spatial pattern recognition, this application eliminates human error, reduces proxy attendance fraud, and provides structured, time-stamped attendance logging.

The application captures frames from local camera streams, pre-processes matrix intensity values, isolates facial coordinates using multi-scale spatial classifiers, and automatically logs verified entries into a persistent database with built-in daily duplicate suppression.

---

## 🏛️ System Architecture & Visual Pipeline

The project implements a modular processing pipeline, separating hardware frame acquisition from facial detection and database write operations:

```text
+-----------------------+
|  Webcam Frame Stream  |  --> Live Capture (Raw BGR Color Matrix)
+-----------+-----------+
            |
            v
+-----------------------+
| Pre-processing Engine |  --> Grayscale Intensity Reduction (cvtColor)
+-----------+-----------+
            |
            v
+-----------------------+
| Spatial Feature Finder|  --> Multi-Scale Feature Classification
+-----------+-----------+
            |
            v
+-----------------------+
| Bounding Box Overlay  |  --> Visual Bounding Box & Identity Rendering
+-----------+-----------+
            |
            v
+-----------------------+
|  Attendance Controller|  --> Duplicate Filtering & Date-Check Logic
+-----------+-----------+
            |
            v
+-----------------------+
|  Persistent Database  |  --> Structured File Storage (attendance.csv)
+-----------------------+