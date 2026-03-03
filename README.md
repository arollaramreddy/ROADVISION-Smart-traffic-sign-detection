# ROADVISION: Smart Traffic Sign Detection using YOLOv8

## Project Overview

ROADVISION is a deep learning-based traffic sign detection and classification system designed for real-world autonomous driving environments.

The system leverages YOLOv8 and Convolutional Neural Networks (CNNs) to achieve high-precision object detection under challenging conditions such as low lighting, occlusion, blur, and noise.

---

## Dataset

- Kaggle Traffic Signs Detection Dataset
- 4,969 real-world traffic sign images
- 15 traffic sign classes
- Standardized resolution: 416×416
- Diverse environments (urban, suburban, highway)
- Varied lighting, weather, and camera angles

---

## Data Preprocessing

- Image resizing and normalization
- Geometric augmentations (rotation, scaling, flipping)
- Photometric adjustments (brightness and contrast)
- Image denoising and sharpening (OpenCV)
- Dataset split: 80% training, 10% validation, 10% testing

---

## Model

- YOLOv8 (Ultralytics implementation)
- Anchor-free object detection
- Transfer learning using pre-trained weights
- Hyperparameter tuning:
  - Batch size: 62
  - Learning rate: 0.01
  - Epochs: 30
  - Optimizer: Auto

---

## Evaluation Metrics

- Precision
- Recall
- mAP@50
- mAP@50–95
- F1-Score

---

## Results

- Precision: 94.22%
- Recall: 90.36%
- mAP@50: 0.962
- mAP@50–95: 0.834
- Peak F1-score: 0.92

The model demonstrated strong real-time detection performance across multiple traffic sign classes, including Stop and Speed Limit signs.

---

## Technologies Used

- Python
- PyTorch
- YOLOv8 (Ultralytics)
- OpenCV
- NumPy
- Matplotlib
