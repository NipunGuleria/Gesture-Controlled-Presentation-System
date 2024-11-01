# Gesture-Controlled-Presentation-System

A computer vision-based system that allows users to control presentations using hand gestures. This project utilizes OpenCV and a hand-tracking module to detect specific hand gestures, which are then mapped to actions like moving to the next or previous slide, zooming, drawing annotations, clearing the screen, and taking screenshots.

## Table of Contents
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Features
- **Navigate Slides**: Move between slides with a swipe left or right gesture.
- **Zoom In/Out**: Use a pinch gesture for zooming.
- **Draw Annotations**: Mark specific points on the slide.
- **Undo/Erase Annotations**: Clear annotations or undo the last action.
- **Screenshot Capture**: Save the current slide as a screenshot.
- **Gesture Recognition**: Recognize gestures such as swipe, pinch, and various finger configurations to control actions.

## Setup
1. Clone this repository:
    ```bash
    git clone https://github.com/NipunGuleria/Gesture-Controlled-Presentation-System
    cd gesture-controlled-presentation
    ```
2. Ensure you have Python 3.7+ and install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Organize slides in a folder named `presentation` within the project directory. Slides should be ordered sequentially by filename.

## Usage
1. Run the main script to start the application:
    ```bash
    python main.py
    ```
2. The webcam will open, and gestures will be detected in real time to control the slides.

### Gesture Controls
- **Previous Slide**: Hold up only the thumb.
- **Next Slide**: Hold up only the pinky finger.
- **Zoom In/Out**: Use pinch gestures with the thumb and index finger.
- **Draw**: Hold up only the index finger.
- **Undo Annotation**: Hold up the index, middle, and ring fingers.
- **Clear Annotations**: Raise all five fingers.
- **Screenshot**: Make a fist.

## How It Works
The application uses the `HandDetector` module to recognize hand gestures from a webcam feed. Each gesture is associated with a specific action, such as slide navigation or zoom. OpenCV is used to manipulate images and annotate slides.

## Dependencies
- `OpenCV`: For handling image and video capture.
- `HandTracker` module: For detecting hand landmarks and gestures.
- `NumPy`: For numerical operations.

## Contributing
1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Submit a pull request.
