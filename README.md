# Hand Tracking Volume Adjuster

<img width="642" height="512" alt="image" src="https://github.com/user-attachments/assets/fce50103-c689-498d-add6-fce7615d93a4" />

Control the system volume on Windows by pinching your thumb and index finger in front of the webcam. Uses MediaPipe for hand tracking and pycaw to talk to the Windows audio endpoint.

## Requirements

- Windows (pycaw is Windows-only)
- Python **3.8 – 3.11 (MediaPipe does not officially support newer versions yet)**
- A webcam

## Libraries

```
opencv-python
mediapipe
numpy
pycaw
comtypes
```

## Usage

Bring your hand in front of the camera. The distance between your thumb tip and index finger tip is mapped to the master volume:

- Fingers close together → mute
- Fingers far apart → max volume

A blue bar on the left shows the current level. Press `Esc` to quit.
