# Bachelor-Thesis-Project-1
# Crack Detection and Quantification using YOLO Framework

This project focuses on the detection and quantification of surface cracks in structures using the YOLO (You Only Look Once) object detection framework. The primary goal is to achieve high accuracy metrics and robust performance to assist in structural health monitoring.

Table of Contents

Introduction

Objectives

Dataset

Methodology

Evaluation Metrics

Results

How to Run

Future Work

Acknowledgments

Introduction

Surface cracks in concrete structures are critical indicators of structural integrity. This project leverages the YOLO framework to detect and quantify these cracks, providing a tool for automated and efficient inspection.

Objectives

Detect surface cracks with high precision and recall.

Quantify cracks to assist in structural assessments.

Optimize the YOLO framework to balance computational efficiency and accuracy.

Dataset

Total Images: Over 1,700 annotated concrete crack images.

Data Annotation: Crack regions annotated using Roboflow to create a YOLO-compatible dataset.

Data Splits:

Training: 70%

Validation: 20%

Testing: 10%

Methodology

Data Preparation:

Annotated images using Roboflow.

Preprocessing included techniques such as CLAHE, Otsu Thresholding, and noise reduction to enhance image clarity.

YOLO Model Training:

Model Used: YOLOv11.

Fine-tuned model parameters for optimal configuration.

Training with variations in background scores (from 1% to 10%) and number of epochs to observe performance trends.

Performance Optimization:

Enhanced detection accuracy through parameter tuning.

Focused on achieving high mAP50 and mAP50-95 metrics.

Evaluation Metrics

mAP@50: Mean Average Precision at IoU threshold of 0.5.

mAP@50-95: Mean Average Precision across IoU thresholds from 0.5 to 0.95.

Precision: Correctly identified cracks / All identified cracks.

Recall: Correctly identified cracks / All actual cracks.

F1 Score: Harmonic mean of precision and recall.

Results

Best Model Metrics:

mAP@50: 92%

mAP@50-95: 77%

Precision: >90%

Recall: >90%

F1 Score: 83%

Object Loss and Box Loss were minimized to acceptable levels during training and validation.

Quantified cracks by their dimensions, providing critical insights for structural assessments.
