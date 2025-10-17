# Deskew Utility (Python + OpenCV)

This script automatically **deskews scanned or photographed documents** by detecting the dominant line orientation and rotating the image back to horizontal alignment.  
It uses **OpenCV** for image preprocessing, noise reduction, thresholding, and **Hough Line Transform** to estimate skew angles.

---

## 🔧 Features
- Automatically detects skewed text or line orientation.
- Handles both **portrait** and **landscape** images.
- Removes small noise using fast non-local means denoising.
- Uses **Otsu’s thresholding** for automatic binary conversion.
- Detects straight lines with the **Probabilistic Hough Transform**.
- Calculates the **median line angle** to correct skew.
- Rotates the image to align horizontally or vertically as needed.

---

## 📦 Dependencies
Install the required Python libraries before running the script:

```bash
pip install opencv-python numpy
