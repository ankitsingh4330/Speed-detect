🚗 Speed Detection using OpenCV
📌 Project Overview

This project detects moving objects using a webcam and estimates their speed in pixels per second (px/s) using computer vision techniques. It uses frame differencing to identify motion and calculates approximate speed based on object movement.

⚙️ Features
Real-time motion detection using webcam
Object detection using contour detection
Speed estimation based on frame rate (FPS)
Bounding box visualization around moving objects
Lightweight and easy to run
🛠️ Technologies Used
Python
OpenCV (cv2)
NumPy
Time module
📂 Project Structure
speeddetect.py   # Main Python script
README.md        # Project documentation
▶️ How It Works
Captures video from webcam
Reads two consecutive frames
Computes difference between frames
Converts to grayscale and applies blur
Applies threshold and dilation
Detects contours (moving objects)

Calculates speed using:

Speed ≈ FPS × (object width / 10)
Displays bounding box and speed on screen
🚀 Installation & Setup
1. Install dependencies
pip install opencv-python numpy
2. Run the project
python speeddetect.py
🖥️ Output
A window named "Speed Detection" will open
Moving objects will be highlighted with a rectangle
Speed will be displayed above the object
⌨️ Controls
Press ESC key to exit the program
⚠️ Limitations
Speed is approximate, not real-world accurate
Works best with stable camera and clear motion
Measures speed in pixels/sec, not km/h
🔮 Future Improvements
Convert speed to real-world units (km/h)
Use object tracking (e.g., YOLO + DeepSORT)
Add multi-object tracking
Improve accuracy with calibration
👨‍💻 Author

Ankit Singh
