# Real-Time Fabric Defect Detection Pipeline

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-ee4c2c.svg)]()

## 📌 Overview
An industrial-grade computer vision pipeline designed to automate textile quality control. Utilizing custom-trained YOLO architectures and PyTorch, this system detects, classifies, and logs fabric anomalies (e.g., mispicks, holes, oil stains) in real-time, operating at latency thresholds suitable for active manufacturing floors.

## 🎯 Objectives
- **Sub-50ms Inference:** Ensure real-time processing speeds compatible with industrial loom outputs.
- **High Recall:** Minimize false negatives to ensure zero-defect downstream manufacturing.
- **Robustness:** Maintain accuracy across variable factory lighting conditions and fabric textures.

## 🛠️ Tech Stack
- **Deep Learning:** PyTorch, YOLOv8
- **Computer Vision:** OpenCV
- **Data Pipeline:** Roboflow (Dataset Augmentation & Annotation)

## 📊 Evaluation Metrics
*(Performance tables including mAP@0.5, Precision, and Recall across various defect classes will be logged here during active training phases).*

## ⚙️ Quick Start
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run inference: `python detect.py --source data/sample_video.mp4 --weights runs/train/exp/weights/best.pt`
