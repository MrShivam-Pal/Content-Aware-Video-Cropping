# Content-Aware-Video-Cropping

## Project Overview

This project implements a content-aware video cropping pipeline using YOLOv8 for object detection and ensures that key objects remain centered in the frame during cropping. The processed video is resized to a target aspect ratio, and audio from the original video is seamlessly integrated into the output.

## Features

Object Detection with YOLOv8: Automatically detects and prioritizes objects in each frame.

Content-Aware Cropping: Crops the video to focus on prioritized objects while maintaining a target aspect ratio.

Temporal Smoothing: Ensures smooth transitions between frames by applying temporal smoothing to cropping coordinates.

Audio Integration: Combines audio from the original video with the processed video.

## Prerequisites

Python 3.8+

The following Python libraries:

OpenCV

ultralytics (YOLOv8)

subprocess (built-in)

FFmpeg installed for audio integration

## Installation

Clone the repository or copy the project files to your local machine.

Install the required Python libraries:

pip install opencv-python ultralytics

Install FFmpeg by following instructions on FFmpeg's official site.

## Usage

Input

Provide an input video file.

Ensure the YOLOv8 model file (e.g., yolov8n.pt) is available.

## Notes

Make sure your system has GPU support if you want to leverage faster processing using YOLOv8.

Use the torch.cuda.is_available() function to verify GPU availability.

FFmpeg must be properly installed for audio integration.

