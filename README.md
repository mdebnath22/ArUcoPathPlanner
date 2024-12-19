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

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/mdebnath22/ArUcoPathPlanner.git
   cd marker-navigation-robot
   ```

2. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Verify Hardware Connections**

   - Ensure your camera and robot are properly connected and configured.

---

## How to Use

### Step 1: Marker Detection

1. Load an image containing ArUco markers:
   ```python
   python detect_markers.py
   ```
2. Visualize the detected markers along with axes and labels.

### Step 2: Coordinate Transformation

- Execute the script to calculate marker positions relative to the screen center:
  ```python
  python calculate_coordinates.py
  ```

## File Structure

```plaintext
├── detect_markers.py        # Marker detection and visualization
├── calculate_coordinates.py # Coordinate mapping and distance calculation
├── requirements.txt         # Python dependencies
├── README.md                # Project overview and instructions
└── images/                  # Example images with markers
```

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

