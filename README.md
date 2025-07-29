# Hand-Gesture-Recognition-System-using-MediaPipe-and-MLP
This project implements a real-time Hand Gesture Recognition System tailored to support physically challenged individuals, enabling them to interact with computers and devices using simple hand movements. The system is built using Python, MediaPipe, and a Multi-layer Perceptron (MLP) model for gesture classification.

## Key Features
Real-time hand tracking using MediaPipe.
Recognizes gestures like:
"I am sick"
"I am in emergency"
"Strangers are in the house"

🔹 Converts gestures into visual and audio outputs using Pygame.

🔹 Designed to empower physically challenged individuals to communicate independently.

🔹 Optimized for use with regular webcams on laptops and smartphones.

## Technologies Used
Tool/Library	Purpose
Python	Programming Language
OpenCV	Image Processing
MediaPipe	Real-time Hand Tracking
Pygame	Audio Feedback
NumPy, Pandas	Data Handling
MLP (Neural Network)	Gesture Classification

## Project Structure
css
Copy
Edit
├── model/
│   ├── keypoint_classifier/
│   │   ├── keypoint_classifier_label.csv
│   │   └── keypoint.csv (training data)
├── music/
│   ├── sick.mp3
│   ├── emergency.mp3
│   └── strangers.mp3
├── main.py  (Gesture Recognition Script)
├── utils.py (Helper Functions)
├── README.md

## How It Works
### Camera Initialization – Captures real-time video.
### Hand Detection – Uses MediaPipe to extract hand landmarks.
### Preprocessing – Normalizes coordinates for consistent model input.
### Gesture Prediction – Classifies gestures using a trained MLP.
### Feedback – Displays gesture on screen and plays corresponding audio message.

## Dataset
The system uses hand landmark data captured via MediaPipe for each gesture and stores them as training data in CSV format. A labeled classifier model is trained using this data for real-time inference.

## Testing Results
High accuracy achieved for key gestures.
Real-time responsiveness observed even on low-spec systems.
Successfully tested on multiple environments (Windows/Linux).

## Future Scope
### Mobile and Embedded Integration: Port to Android/iOS or Raspberry Pi.
### Gesture-based Gaming: Use gestures for immersive experiences.
### More Gestures: Extend system to recognize sign language alphabets and numbers.

## References
MediaPipe Framework
Pygame Documentation
CNN & MLP Concepts
Hand Gesture Recognition Papers and Surveys

### Getting Started
To run the system:
bash
Copy
Edit
pip install opencv-python mediapipe pygame numpy pandas
python main.py

### This project was developed as part of an academic initiative by the Department of Computer Science, SSC, Shimoga, aiming to build accessible AI-driven tools for inclusive technology.
