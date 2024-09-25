# Virtual Mouse Using Fingers with Python and OpenCV
This project demonstrates how to control the mouse cursor using finger movements tracked by a webcam. The project uses Python and OpenCV to process real-time video, detect hand gestures, and move the cursor accordingly. The goal is to create a simple, efficient, and intuitive virtual mouse system

## Features

* ### **Hand and Finger Detection:** Uses OpenCV to detect the user's hand and track specific finger movements.
* ### Cursor Control: Move the mouse cursor by detecting the position of the index finger.
* ### Click Events: Simulate left and right mouse clicks using different finger gestures.
* ### Gesture-Based Control: Other gestures can be mapped to different functionalities (e.g., scrolling, dragging).

  # Requirements
* Python 3.x
* OpenCV (cv2)
* MediaPipe (mediapipe)
* PyAutoGUI (pyautogui)

  ## Code:
```
pip install opencv-python mediapipe pyautogui
```

# How it Works
1. Hand Detection: The project uses MediaPipe to identify the user's hand in real-time video. It locates key landmarks on the hand (such as finger tips and knuckles).
2. Finger Tracking: The landmarks of the index and middle fingers are used to track the movement of the fingers and translate that into mouse movements. The distance between fingers can also be used to simulate mouse clicks.
3. Mouse Control: Using the pyautogui library, finger movements are translated into actions on the screen. The index finger controls the cursor's position, and gestures involving the thumb and other fingers trigger click or scroll actions.

# Key Functions
* Index Finger Movement: Controls the movement of the cursor.
* Pinch Gesture: Thumb and index finger together simulate a left-click.
* Three Finger Gesture: Move three fingers together to scroll the window up or down.
* Index and Middle Finger Gesture: Hold both fingers up to simulate right-click

# Demo
Here’s a simple demo of how the project works:

[![Demo]("C:\Users\ymrat\OneDrive\Desktop\VID-20240510-WA0000.mp4")]


# Known Issues
* Lighting Conditions: The accuracy of hand detection may vary depending on the lighting conditions.
* Webcam Resolution: Using a low-quality webcam can reduce detection accuracy and response time.
* CPU Usage: Real-time video processing can be resource-intensive; using a more powerful computer may improve performance.

# Future Improvements
* Improved gesture recognition for additional control features.
* Enhanced stability and reduced latency for smoother control.
* Integration with additional gesture-based libraries for more functionalities.


# If you find this project helpful, consider giving it a ⭐ on GitHub!
  
