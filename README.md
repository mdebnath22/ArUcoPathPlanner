# ArUco Marker Navigation and Path Planning with MyCobot 600 Pro

## Overview

This project implements a system to detect ArUco markers and calculate their relative positions, translating the data into robot-coordinated movements. It integrates image processing, marker detection, and transformation matrix computations to facilitate navigation from one marker to another using a robotic system.

---

## Features

- **ArUco Marker Detection:** Detects and identifies ArUco markers in a provided image.
- **Coordinate Mapping:** Maps detected markers' coordinates to a custom coordinate system centered at the screen's origin.
- **Distance Calculation:** Converts pixel coordinates to real-world millimeters using a known scale.
- **Homogeneous Transformation:** Employs forward kinematics for precise robot end-effector positioning.

---

## Prerequisites

### Hardware

- Camera for capturing marker images
- Compatible robotic arm or robot

### Software

- Python 3.8+
- Required Python libraries: OpenCV, NumPy, Matplotlib, SciPy
- MATLAB (for kinematics and optimization tasks)

---

## Outputs

- **Relative Coordinates:** Coordinates of detected markers relative to the screen origin.
- **Converted Coordinates:** Marker coordinates in millimeters for robot navigation.
- **Robot Movements:** Joint angles for optimized end-effector positioning.

---

## Example Workflow

1. Detect ArUco markers in a maze-like environment.
2. Calculate real-world distances between markers.
3. Translate the data into robot-coordinated movements.
4. Use the robot to navigate from one marker to another.

---

For questions or contributions, please open an issue or submit a pull request!

