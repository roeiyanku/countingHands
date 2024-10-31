# Real-Time Finger Counting using OpenCV and MediaPipe

This project detects the number of fingers held up in real-time using OpenCV for video capture and MediaPipe for hand landmark detection.

## Features

- **Real-Time Finger Counting**: Detects hand landmarks and counts raised fingers.
- **On-Screen Display**: The number of raised fingers is displayed directly on the video feed.

## Requirements

- **Python 3.x**
- **Packages**: `opencv-python`, `mediapipe`

## Installation

Install the required packages with:
```bash
pip install opencv-python mediapipe
```

## Usage

1. **Run the Script**:
   ```bash
   python finger_counter.py
   ```
2. **Video Capture**: Make sure your webcam is functional and enabled, as the script will open a video feed.

3. **Finger Counting**:
   - A count of the raised fingers appears on the screen, updating in real-time as you hold up or lower fingers.

## Code Overview

- **Modules**:
  - `cv2.VideoCapture(0)`: Captures video from the default webcam.
  - `mediapipe.solutions.hands`: Detects hand landmarks and connections.
  - `fingerCoordinates` and `thumbCoordinate`: Store landmark indices used for determining if fingers are raised.

- **Main Loop**:
  - The script reads frames from the webcam, detects hand landmarks, and counts raised fingers based on the relative position of specific hand landmarks.

## References

- **OpenCV**: [Documentation](https://opencv.org/)
- **MediaPipe**: [Documentation](https://google.github.io/mediapipe/)

---

This script is a useful starting point for gesture recognition applications and provides hands-on experience with hand landmark detection and video processing in Python.
