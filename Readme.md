# Run TensorFlow Lite Models on Windows

Follow these steps to set up and run TensorFlow Lite models on a Windows machine.

## Prerequisites
- Ensure you have a **USB webcam** plugged into your computer, or use a laptop with a built-in camera.

## Steps to Set Up

### 1. Download and Install Anaconda
Download and install Anaconda from the official website: [https://www.anaconda.com/](https://www.anaconda.com/).

### 2. Set Up the Environment
Using the Anaconda Command Prompt, run the following commands to create a dedicated environment for TensorFlow Lite:
```bash
mkdir C:\tflite1
cd C:\tflite1
conda create --name tflite1-env python=3.9
conda activate tflite1-env
pip install tensorflow opencv-python protobuf==3.20.*
```

# `Running TensorFlow Lite Models`
**Webcam Detection**
python TFLite_detection_webcam.py --modeldir=TFLite_model

**Video Detection**
To run object detection on a video file, use the following command:
python TFLite_detection_video.py --modeldir=TFLite_model
