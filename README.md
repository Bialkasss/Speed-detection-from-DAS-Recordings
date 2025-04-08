# 🚌 Moving Objects Detection in DAS Recordings 🚊

![DAS Detection](https://img.shields.io/badge/Computer%20Vision-Acoustic%20Sensing-blue)
![Python](https://img.shields.io/badge/Python-3.7+-yellow)
![OpenCV](https://img.shields.io/badge/OpenCV-4.5+-green)

## 📋 Project Overview

This project detects moving objects (vehicles like trams, trucks, and cars) in Distributed Acoustic Sensing (DAS) data collected from fiber optic cables under a street. The algorithm identifies characteristic slanted lines in the time-space domain and calculates vehicle velocities.

## ⚙️ Algorithm Pipeline

1. **Preprocessing**
   - Resize
   - Apply MinMax normalization
   - Handle outliers

2. **Denoising**
   - Median blur
   - Enhancing signals using power transformation
   - Thresholding

3. **Morphological Processing**
   - Binarize
   - Apply morphological closing
   - Erode 

4. **Line Detection & Analysis**
   - Apply Hough Transform
   - Group and merge related line segments
   - Convert pixel coordinates to physical dimensions
   - Calculate vehicle velocities

## 🚀 Results

The algorithm successfully detects moving objects in all test datasets despite varying noise conditions. The technique correctly identifies vehicles moving at different speeds and directions.

## 👩‍💻 Authors

- Maria Musiał 
- Martyna Stasiak 
