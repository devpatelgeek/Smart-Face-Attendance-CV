# Problem Statement: Computer Vision Based Automated Face Attendance System

## Problem Statement
Traditional classroom and workplace attendance tracking methods rely heavily on manual sign-in sheets or physical roll calls. These manual approaches are time-consuming, disrupt workflow efficiency, and are susceptible to proxy attendance abuses.

## Scope of Project
This project designs and implements an automated vision processing pipeline. Using digital image processing techniques and OpenCV's Haar Cascade spatial feature extractors, the application detects human facial structures from live video feeds and automatically logs unique, timestamped attendance records into a structured local database.

## Target Users
- **Educational Faculty & Instructors:** To capture automated, non-intrusive student presence logs.
- **Enterprise Administrators:** To maintain automated access logs for physical premises.

## High-Level Features
- Real-time video frame acquisition and color-space conversion (BGR to Grayscale).
- Spatial boundary detection and dynamic bounding-box overlay rendering.
- Automated non-duplicate logging logic filtering multiple detections within the same day.
- Flat CSV storage persistent backend for auditability.