# 👁️ Smart Automated Face Attendance System (Computer Vision)

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Data Integrity](https://img.shields.io/badge/Database-CSV%20Logging-green?style=for-the-badge)

🚀 **Overview**

This project is a high-performance **Computer Vision application** built to automate attendance tracking using real-time face detection and spatial pattern recognition. It replaces slow, error-prone manual roll calls with an automated vision processing pipeline, logging timestamped entries to a persistent storage system while preventing duplicate logging.

---

## ✨ Key Features

- 📹 **Real-Time Video Stream Pipeline:** Processes live frames from hardware capture devices cleanly.
- 🎯 **Multi-Scale Spatial Detection:** Utilizes spatial feature extraction for human face detection.
- ⚡ **Automated Log Prevention:** Smart duplicate entry detection per calendar date.
- 📂 **Persistent Audit Backend:** Automatic logging to structured CSV flat-file databases.
- 🧱 **Modular Architecture:** Clean separation of vision capture logic and database persistence.

---

## 🏗️ Project Structure

```text
Smart-Face-Attendance-CV/
│
├── main.py              # Main execution script & vision pipeline simulation
├── attendance.csv       # Persistent timestamped database log
├── statement.md         # Detailed Problem Statement & Project Scope
├── requirements.txt     # System dependency management file
└── README.md            # Comprehensive project documentation