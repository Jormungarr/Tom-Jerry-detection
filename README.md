# Tom & Jerry Detection (YOLOv8 Toy Project)

> A lightweight toy project for detecting **Tom** and **Jerry** in images using **YOLO (Ultralytics YOLOv8)**.

## Overview
This repository demonstrates a minimal end-to-end object detection pipeline:
- **Data**: custom-labeled images of Tom & Jerry
- **Model**: YOLOv8 (Ultralytics)
- **Tasks**: train → validate → inference → visualization
- **Goal**: build a clean, reproducible baseline and visualize prediction quality

**Why YOLO?**  
YOLO (You Only Look Once) is a one-stage object detector that predicts bounding boxes and class probabilities in a single forward pass, making it fast and practical for real-time or near real-time detection.

---

## Features
- ✅ Train YOLOv8 on a small custom dataset (Tom/Jerry)
- ✅ Run inference on images
- ✅ Visualize predicted bounding boxes + confidence scores
- ✅ Export results for inspection (optional: CSV/JSON)

---

## Demo
> Put your best qualitative results here.

<p align="center">
  <img src="assets/demo_1.jpg" width="80%" />
</p>

<p align="center">
  <img src="assets/demo_2.jpg" width="80%" />
</p>

> If you have a GIF:
<!-- <p align="center">
  <img src="assets/demo.gif" width="80%" />
</p> -->

---

## Project Structure
```text
.
├── data/                      # dataset (or link / instructions)
│   ├── images/
│   │   ├── train/
│   │   └── val/
│   └── labels/
│       ├── train/
│       └── val/
├── runs/                      # YOLO training outputs (usually gitignored)
├── assets/                    # README images/GIFs
├── scripts/                   # helper scripts (train/infer/viz)
├── yolov8.yaml                # dataset config (or data.yaml)
├── requirements.txt
└── README.md
