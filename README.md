Gesture Based Volume Control Using Hand Gestures

📌 Project Overview:
This project implements a gesture-based system volume controller using hand gestures captured through a webcam. By measuring the distance between specific hand landmarks, the system dynamically increases or decreases the system volume without any physical contact.

The project uses Computer Vision and Hand Tracking to provide a touch-free and intuitive user experience.

🚀 Features:
Real-time hand gesture recognition using a webcam
Touchless system volume control
Smooth and responsive volume adjustment
Interactive UI using Streamlit
Visual feedback for hand landmarks and gesture distance

🛠️ Technologies & Libraries Used:
OpenCV – Live webcam video capture and frame processing
MediaPipe – Hand detection and 21 hand landmark tracking
PyAutoGUI – Controlling system volume programmatically
Streamlit – Web-based UI for running and visualizing the project
NumPy – Numerical computations and distance calculations
Plotly – Visualization and interactive graphs

✋ Hand Gesture Logic:
MediaPipe detects 21 hand landmarks, including fingertips
Distance is calculated between selected landmarks (e.g., thumb tip and index finger tip)
Minimum distance: 0
Maximum effective distance: 150
Volume Mapping:
Increasing the distance between fingers → Volume increases
Decreasing the distance between fingers → Volume decreases
If the distance exceeds 150 (e.g., 250), the volume remains capped at 100%
Volume scales smoothly within the defined distance range

⚙️ Working Principle:
Webcam captures live video feed
OpenCV processes video frames
MediaPipe identifies hand landmarks
Distance between landmarks is calculated using NumPy
Distance is mapped to system volume level
PyAutoGUI adjusts the system volume accordingly
Streamlit displays real-time feedback and visualization
