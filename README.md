# SAFETY-EQUIPMENT-DETECTION-USING-YOLOv5-FOR-INDUSTRIAL-SURVEILLANCE


## Overview

This project aims to develop an AI-powered system for detecting safety equipment on workers in industrial environments such as oil rigs, refineries, and construction sites. Using **YOLOv5**, a state-of-the-art object detection model, the system automatically identifies whether personnel are wearing essential safety gear like helmets, vests, gloves, and masks, enhancing workplace safety and compliance monitoring.

---

## Features

- Real-time detection of multiple safety equipment types  
- High accuracy and fast inference using YOLOv5  
- Can be integrated with surveillance cameras for continuous monitoring  
- Alerts for missing or improper safety gear  
- Supports static images  

---

## Dataset

The model is trained on the **Roboflow PPE Dataset**, which includes annotated images of workers wearing various safety equipment. Data augmentation techniques were used to improve model robustness.

---

## Technologies Used

- Python  
- PyTorch  
- YOLOv5 (Ultralytics implementation)  
- OpenCV for image/video processing  
- Roboflow Dataset for training data  
- Google Colab (optional) for training and testing  

---

## 📊 Model Evaluation Metrics
After training the YOLOv5 model for 50 epochs, the following evaluation metrics were obtained:

| **Metric**        | **Value** |
| ----------------- | --------- |
| **Precision (P)** | 0.818     |
| **Recall (R)**    | 0.632     |
| **mAP\@0.5**      | 0.682     |
| **mAP\@0.5:0.95** | 0.317     |

Precision measures the model’s accuracy in correctly identifying safety equipment (PPE), minimizing false positives.

Recall reflects the model’s ability to detect all actual PPE instances, minimizing false negatives.

mAP (mean Average Precision) is a standard object detection metric evaluating both precision and recall across different thresholds.

mAP@0.5: Average precision at Intersection over Union (IoU) threshold of 0.5.

mAP@0.5:0.95: Average precision averaged over multiple IoU thresholds (more stringent evaluation).


