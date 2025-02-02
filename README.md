# Hand Tracking and Segmentation with MediaPipe, Ultralytics, and SAM 2

This project implements **hand tracking and segmentation** using OpenCV, MediaPipe, Ultralytics YOLO, and SAM 2 (Segment Anything Model). It processes a video file, detects hands, and applies segmentation, saving the output with tracked hand landmarks and masks.

## Features
- Reads an input video file
- Detects hands using **MediaPipe**
- Draws hand landmarks on each frame
- Applies segmentation using **Ultralytics YOLO and SAM 2**
- Saves the processed video with hand tracking and segmentation masks

## Installation
### Prerequisites
Ensure you have Python installed, then install the required dependencies:
```bash
pip install opencv-python mediapipe ultralytics segment-anything torch
```

## Usage
1. Place your video file (`test.mp4`) in the same directory as the script.
2. Run the script:
```bash
python hand_track.py
```
3. The output video will be saved as `output_hand_tracking.mp4`.

## How It Works
- **Loads the video** file using OpenCV.
- **Uses MediaPipe Hands** to detect and track hand landmarks.
- **Draws hand connections** on the frames.
- **Applies SAM 2 segmentation** to generate masks around detected hands.
- **Overlays masks** on the video.
- **Writes the processed frames** to an output video file.
- **Allows real-time display** of the video and stops when 'Q' is pressed.

## Output
The processed video is saved as `output_hand_tracking.mp4` in the same directory.

