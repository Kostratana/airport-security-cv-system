# Airport Security AI System

> Applied Computer Vision project focused on real-world airport security systems.

Computer vision system for detecting prohibited items in X-ray scans using deep learning (YOLO-based models).

---

## Overview

This project implements an AI-based solution for automated detection of dangerous and prohibited objects in X-ray images used in airport security screening.

The system was developed as part of a real-world security task and aims to improve the efficiency, consistency, and reliability of passenger inspection processes.

---

## Key Features

- Object detection using YOLOv8  
- Additional experiments with Keras CV models  
- Custom dataset of annotated X-ray images  
- Data preprocessing and augmentation using OpenCV  
- Model evaluation using precision, recall, and mAP metrics  
- Comparative analysis of multiple training configurations  

---

## Dataset

- ~9,000+ processed and augmented images  
- Annotated using CVAT  

Includes:
- normal passenger scans  
- prohibited and dangerous objects  

Preprocessing:
- grayscale conversion  
- dataset augmentation (multiple variations per image)  
- dataset balancing  

---

## Experiments

The project includes experimental evaluation of multiple model configurations:

- YOLOv8 (extended training ~100 epochs)  
- YOLOv8 (short training ~30 epochs)  
- Keras CV YOLO-based detector  

The goal was to analyze trade-offs between detection accuracy, generalization, and training efficiency.

---

## Results

Best model performance:

- Precision: ~61.6%  
- Recall: ~36.8%  
- mAP@0.5: ~40.7%  

### Observations

- Longer training improved detection performance  
- Overfitting was observed in some configurations  
- Keras CV models showed weaker generalization compared to YOLOv8  
- Dataset quality and augmentation significantly impacted results  

---

## Tech Stack

- Python  
- YOLOv8 (Ultralytics)  
- TensorFlow / Keras CV  
- OpenCV  
- CVAT (annotation tool)  

---

## Research & Experiments

This project follows an experimental approach to model development:

- multiple training strategies were tested  
- configurations were compared using standard CV metrics  
- results were analyzed to guide further improvements  

---

## Future Work

- Improve generalization and reduce overfitting  
- Expand dataset with more diverse samples  
- Optimize model architecture and hyperparameters  
- Deploy as a real-time security inspection system  

---

## Author

Svetlana Rumyantseva  
AI Systems Engineer  
