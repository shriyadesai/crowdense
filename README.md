# Crowdness Prediction and Monitoring System

This project is designed to predict and monitor crowd density in a specific area using real-time camera feeds. It uses a deep learning-based object detection model and centroid tracking to monitor people entering and exiting the area, providing real-time crowd analysis and alerts when crowd density exceeds a defined threshold.

## Features
- **Real-time crowd density prediction** using object detection and tracking.
- **Centroid tracking** to accurately follow individuals across frames.
- **Email alerts** when crowd density exceeds a predefined threshold.
- **Automatic logging** of crowd data to a CSV file.
- **Supports live IP camera streams or video file inputs**.
- **FPS tracking** for performance evaluation.
- **Configurable scheduler** to automatically run and stop the system.

## Prerequisites

- Python 3.x
- OpenCV
- Dlib
- Imutils
- NumPy
- Caffe (for deep learning model)
- A trained model (such as MobileNet SSD) for object detection.

## Installation

1. Clone the repository and install the required Python libraries:
2. Ensure you have the Caffe model and its corresponding prototxt file for MobileNet SSD. You can download them from the official sources if not provided.

## Usage

### Running the System

To run the system, you need to pass the path to the pre-trained model, the prototxt file, and optionally an input video file or a live camera feed:

```bash
python crowdness_predictor.py --model <path_to_model> --prototxt <path_to_prototxt> --input <optional_input_video> --output <optional_output_video>

