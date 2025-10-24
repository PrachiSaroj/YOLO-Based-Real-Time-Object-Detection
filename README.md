# YOLO-Based-Real-Time-Object-Detection
A real-time computer vision system that detects objects using YOLOv5 and webcam input for live object tracking and analysis.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Configuration & Models](#configuration--models)
- [Potential Improvements](#potential-improvements)
- [Project Files](#project-files)
- [License & Credits](#license--credits)
- [Contact / Contributors](#contact--contributors)

## Overview

This project enables **real-time object detection** using a webcam. YOLOv5 identifies objects in the camera feed and displays bounding boxes with labels for each detected object.

## Features

- Real-time object detection from webcam input.  
- Draws bounding boxes with labels for detected objects.  
- Lightweight and efficient; can run on CPU or GPU.  
- Easily configurable YOLO model weights and detection parameters.

## Tech Stack

- **Programming Language:** Python  
- **Libraries:** OpenCV, PyTorch, YOLOv5, NumPy  
- **Environment:** Google Colab / Jupyter Notebook (optional for prototyping)  

## Requirements

- Python 3.8+  
- OpenCV (`opencv-python`)  
- PyTorch (compatible with your CPU or CUDA version)  
- YOLOv5 repository (cloned from [Ultralytics](https://github.com/ultralytics/yolov5))  
- NumPy  

Install dependencies using pip:
pip install opencv-python torch torchvision numpy

## How It Works

1. **Capture frames** from the webcam using OpenCV.  
2. **Load YOLOv5 model weights** and perform object detection on each frame.  
3. **Draw bounding boxes and labels** around detected objects.  
4. **Display annotated frames** in a live window.  
5. **Continue detection in real-time** until the user exits the program.

## Configuration & Models

- **models/** : Contains YOLO model weights (e.g., `yolov5s.pt`).  
- **run_object_detection.py** : Main script to run real-time detection.  
- **Custom models (optional):** You can fine-tune YOLOv5 on a custom dataset and place the resulting `.pt` file in the `models/` folder for use in the project.

## Potential Improvements

- **Multiple input sources:** Add support for multiple cameras or video file input.  
- **Object tracking:** Integrate with tracking algorithms for smoother detection across frames.  
- **Alert notifications:** Expand functionality to include alerts when certain objects are detected.  
- **Performance optimization:** Optimize the model for faster performance on CPU.

## Project Files

- `run_object_detection.py` — Main script for real-time object detection  
- `models/` — Folder containing YOLOv5 model weights  
- `requirements.txt` — Python dependencies  
- `notebooks/` — Optional Colab notebooks for prototyping  

## License & Credits  

- **Credits:** Built using OpenCV, Ultralytics YOLOv5, PyTorch, and other open-source resources

## Contact / Contributors

- **Author:** Prachi Saroj  
- **Email:** prachisaroj11@gmail.com  

Contributions are welcome — open an issue or submit a pull request with improvements.



