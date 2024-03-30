# Fruit Inspection - IPCV Project

## Introduction
This project is aimed at inspecting fruits, specifically apples, for defects and russet regions using computer vision techniques. The project is structured into two main tasks: defect detection and russet region detection across different color spaces.

## Overview
- **Task A**: Focuses on identifying external defects such as bumps, holes, or indentations on the surface of apples using image processing techniques.
- **Task B**: Aims at detecting russet defects on apples, employing a Mahalanobis distance function across different colour spaces.

## Task A: Fruit Segmentation and Defect Detection
This task employs several image-processing techniques to identify defects:
1. **Grayscale Histogram Analysis** to find optimal thresholding values.
2. **Gaussian Smoothing** to reduce noise.
3. **Otsu's Thresholding** for improved binarization, highlighting defects.
4. **Sobel and Canny Edge Detection** to identify the edges of defects.
5. **Morphological Operations** (Erosion and Dilation) to isolate defect edges.

### Results for Task A
- Successful identification and filling of defect holes in most images.
- Major defect marks were detected accurately, except for certain areas where adjustment of threshold values was needed.


## Task B: Russet Region Detection
Task B implements the following steps to detect russet regions:
1. **Grayscale Histogram Analysis** and **Gaussian Smoothing** for initial thresholding.
2. **Manual and Otsu's Thresholding** to generate a binary mask for colour space analysis.
3. **Color Space Conversion** to HSV, HLS, and LUV for detailed inspection.
4. **Mahalanobis Distance Calculation** to identify russet regions based on colour deviations.

### Results for Task B
- Russet regions were successfully marked in one of the images with significant accuracy using the LUV colour space.
- Manual selection of regions of interest (ROI) was required for precise detection.

## Code Usage
The project includes Jupyter Notebooks (`Part1.ipynb` for Task A and `Part2.ipynb` for Task B) that demonstrate the methodology and results for each task.
