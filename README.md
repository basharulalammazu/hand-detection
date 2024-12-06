# Hand Detection with MediaPipe and OpenCV

This project leverages **OpenCV** and **MediaPipe** to perform real-time hand detection through a webcam, displaying hand landmarks with FPS (Frames Per Second) information. The application continuously captures video from the default camera, processes it using MediaPipe’s hand detection model, and visualizes the output by drawing landmarks on the hands.


## Overview

This Python application uses **OpenCV** for video capture and **MediaPipe** for detecting hand landmarks. The script runs a loop that captures video from the camera, converts each frame to RGB format, and uses the MediaPipe API to process the frame for hand landmarks. The FPS of the video stream is displayed in the top-left corner of the output window.

The project is intended for use in applications requiring hand gesture recognition or hand tracking, and can be easily modified or extended for various use cases, such as sign language recognition, virtual interfaces, or interactive installations.

## Installation

Follow these steps to set up the project on your local machine:

### Step 1: Install Python

Ensure you have Python 3.x installed. You can download it from the official Python website:  
[Download Python](https://www.python.org/downloads/).

### Step 2: Install Required Libraries

The project relies on two primary libraries: `OpenCV` for video capture and image processing, and `MediaPipe` for hand landmark detection. Install them using `pip`:

```bash
pip install opencv-python mediapipe
```

Note: The `time` module is part of Python's standard library and does not require installation.

### Step 3: Clone the Repository (Optional)

If you'd like to download this project for local use, clone the repository using Git:

```bash
git clone https://github.com/basharulalammazu/hand-detection.git
cd hand-detection
```

### Step 4: Run the Script

Once the dependencies are installed, run the Python script to start the hand detection application:

```bash
python hand_detection.py
```

Ensure your camera is connected and accessible before running the script.

## Usage

### How It Works:
1. **Video Capture**: The application accesses the default camera and captures real-time video.
2. **Hand Detection**: Each frame is processed by the **MediaPipe Hands API** to detect hand landmarks. If hands are detected, the landmarks are drawn on the video feed.
3. **FPS Calculation**: The application calculates the Frames Per Second (FPS) based on the time between successive frames and displays it on the video feed.
4. **Real-time Display**: The processed video, with hand landmarks and FPS information, is displayed in a new window.

### Exit the Program:
To close the application, press the **`q`** key while the video window is active.

## Features

- **Real-time Hand Landmark Detection**: Uses **MediaPipe** for robust and efficient hand detection in live video.
- **FPS Monitoring**: Displays the FPS in the top-left corner of the video window to monitor performance.
- **Camera Access**: Supports accessing and using the default webcam on the system for video capture.
- **Customizable**: The script can be easily extended for more advanced hand gesture recognition or used as a basis for interactive applications.

## Dependencies

This project requires the following Python packages:

- **OpenCV**: For capturing video and processing images.
  - Install via `pip install opencv-python`
  
- **MediaPipe**: For hand landmark detection and visualization.
  - Install via `pip install mediapipe`

- **time**: Part of Python’s standard library, used for FPS calculation.

To install the dependencies, you can run the following command:

```bash
pip install opencv-python mediapipe
