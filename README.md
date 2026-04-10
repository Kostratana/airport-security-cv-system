# Airport Security AI System

Computer vision system for detecting prohibited items in X-ray scans for airport security screening.

---

## Overview

This project implements an AI-based system for automated detection of dangerous and prohibited objects in X-ray images used in airport security.

The system was developed as part of a real-world task in the security domain and focuses on improving the efficiency and reliability of passenger screening processes.

---

## Key Features

- Object detection using YOLOv8  
- Additional experiments with Keras CV models  
- Custom dataset with annotated X-ray images  
- Data preprocessing using OpenCV  
- Model evaluation using precision, recall, and mAP metrics  
- Comparative analysis of different training configurations  

---

## Dataset

- ~9,000+ images (processed and augmented)  
- Annotated using CVAT  

Includes:
- normal passenger scans  
- prohibited / dangerous objects  

Preprocessing:
- grayscale conversion  
- multiple augmented copies per image  
- dataset balancing  

---

## Experiments

Multiple model configurations were trained and evaluated:

- YOLOv8 (extended training, ~100 epochs)  
- YOLOv8 (short training, ~30 epochs)  
- Keras CV YOLO-based detector  

---

## Results

Best model performance:

- Precision: ~61.6%  
- Recall: ~36.8%  
- mAP@0.5: ~40.7%  

Observations:

- Longer training improved detection quality  
- Validation results indicated overfitting in some configurations  
- Keras CV model showed weaker generalization compared to YOLOv8  
- Dataset quality and augmentation strongly influenced results  

---

## Tech Stack

- Python  
- YOLOv8 (Ultralytics)  
- TensorFlow / Keras CV  
- OpenCV  
- CVAT (annotation tool)  

---

## Future Work

- Improve generalization and reduce overfitting  
- Expand dataset with more diverse samples  
- Optimize model architecture and hyperparameters  
- Deploy system for real-time security screening  

---

## Author

Svetlana Rumyantseva  
AI Systems Engineer  
