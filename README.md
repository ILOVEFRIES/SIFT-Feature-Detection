# SIFT Feature Matching using OpenCV

_Based on Chapter 5 — Practical Machine Learning and Image Processing for Facial Recognition, Object Detection, and Pattern Recognition Using Python (Himanshu Singh)_

---

## Project Overview

This project demonstrates the use of the **Scale-Invariant Feature Transform (SIFT)** algorithm to detect and match features between two images.

SIFT is a computer vision algorithm that identifies distinctive keypoints and descriptors that remain consistent even when the images are captured at different scales, rotations, or lighting conditions.

---

## Technologies Used

- **Python 3.x**
- **OpenCV (cv2)**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**

---

## How It Works

1. **Read two input images** (e.g., `pantheon1.jpg` and `pantheon2.jpg`).
2. **Convert both images to grayscale.**
3. **Detect SIFT keypoints and compute descriptors** using:
   ```python
   sift = cv2.SIFT_create()
   keypoints, descriptors = sift.detectAndCompute(gray, None)
   ```
