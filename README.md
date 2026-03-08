# ARK_PERCEPTION_CV_TASK_2.2
Task 2.2 – Noise Filtering
Objective

The goal of this task is to remove high-frequency salt noise from corrupted images while preserving the important features of the image such as edges and structures.

Input Images

iron_man_noisy.jpg

scenary_noise.jpg

Approach

The following image processing pipeline was used:

Load the noisy image using OpenCV

Convert the image to grayscale

Apply Median Filtering to remove salt noise

Use Morphological Opening to remove remaining artifacts

Save the processed clean image

Key Concepts

Salt-and-pepper noise removal

Median filtering

Morphological image processing

Output

The final images show significant noise reduction while preserving the original line structure.
