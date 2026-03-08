# ARK_PERCEPTION_CV_TASK

ARK Perception Team – Computer Vision Tasks

This repository contains my solutions for the ARK Perception Team Selection Tasks (Computer Vision).
The objective of these tasks is to apply image processing and computer vision techniques to solve practical problems involving noise removal and geometric feature detection.

The tasks were implemented using Python, OpenCV, NumPy, and Jupyter Notebook.

Tasks Implemented
Task 2.2 – Noise Filtering
Objective

The goal of this task is to restore corrupted images affected by high-frequency salt noise (random white pixels) while preserving important visual features such as edges and line structures.

Approach

The following image processing pipeline was implemented:

Load the noisy images using OpenCV

Convert the image to grayscale

Apply Median Filtering to remove salt noise

Use Morphological Opening to remove remaining artifacts

Save the processed image

Key Concepts Used

Salt-and-pepper noise removal

Median filtering (non-linear filter)

Morphological operations (erosion and dilation)

Result

The processed images show:

Significant reduction of noise

Preservation of line structures

Improved visual clarity

Task 2.3 – Medial Axis Detection of Moving Objects
Objective

The objective of this task is to detect the medial axis (central skeletal line) of a moving surgical tool in a video sequence.

The medial axis represents the geometric center of an object and is useful for analyzing its orientation and structural properties.

Processing Pipeline

The following computer vision pipeline was implemented:

Frame Extraction
Extract frames from the input video.

Background Subtraction
Separate the moving object from the static background.

Morphological Cleaning
Remove noise and fill small gaps using erosion and dilation.

Edge Detection
Detect object boundaries using Sobel derivatives.

Custom Hough Line Transform
Detect straight edges of the tool using a manually implemented Hough Transform.

Medial Axis Computation
Compute the central axis between the detected edges.

Visualization
Overlay the detected medial axis on the original video frames.

Important Constraint

The Hough Transform was implemented from scratch without using OpenCV’s built-in Hough transform functions.

Result

The algorithm successfully detects the edges of the tool and computes the central skeletal axis, which is visualized on the video frames.

Technologies Used

Python

OpenCV

NumPy

Matplotlib

Jupyter Notebook
