Currently in development
hosted at : https://awshae.github.io/FFUAV/

# FFUAV – Autonomous Fire-Fighting UAV System

An end-to-end autonomous emergency response drone system built using **ROS2, ArduPilot, Firebase, and AI-based perception**.

This project enables real-time civilian emergency reporting, autonomous mission dispatch, live tracking, and intelligent onboard processing.

---

## System Overview

The system consists of three major layers:

### Public Emergency Interface
- Web-based alert submission (Leaflet + Firebase)
- Location selection (map click or GPS)
- Severity classification
- Real-time system lock when drone is deployed

### Admin Command Center
- Live mission monitoring
- Deploy / Abort control
- Drone telemetry tracking
- Firestore-based command pipeline
- Auto system unlock on mission completion

### UAV Stack
- **Pixhawk (ArduPilot 4.6)** – Flight control
- **ROS2** – Mission orchestration
- **MAVROS** – MAVLink bridge
- **Raspberry Pi 5** – Companion computer
- AI inference pipeline (YOLO-based detection ready)
- Firestore bidirectional sync
---
## Architecture
Civilian → Firebase → Admin → Firestore Command → ROS2 Controller → MAVROS → ArduPilot → Drone  
Telemetry → ROS2 → Firestore → Admin Dashboard
---
## Tech Stack
### Flight Stack
- ROS2 (Humble)
- MAVROS
- ArduPilot 4.6
- Gazebo Harmonic (Simulation)
### Web Stack
- HTML + CSS
- Leaflet.js
- Firebase Firestore (Realtime DB logic)
### Hardware
- Pixhawk 2.4.8
- Raspberry Pi 5 16GB
- Oak-d lite depth camera
---

