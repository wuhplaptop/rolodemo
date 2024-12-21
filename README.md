# smalltestupload

## Model Overview

**Architecture:** YOLOv11  
**Training Epochs:** 50  
**Batch Size:** 32  
**Optimizer:** auto  
**Learning Rate:** 0.0005  
**Data Augmentation Level:** Moderate

## Training Metrics

- **mAP@0.5:** 0.995

## Class IDs

| Class ID | Class Name |
|----------|------------|
| 0 | Panadol |
| 1 | Revanin |


## Description

This model was trained using the YOLOv11 architecture on a custom dataset. The training process involved 50 epochs with a batch size of 32. The optimizer used was **auto** with an initial learning rate of 0.0005. Data augmentation was set to the **Moderate** level to enhance model robustness.

## Usage

To use this model for inference, follow the instructions below:

```python
from ultralytics import YOLO

# Load the trained model
model = YOLO('best.pt')

# Perform inference on an image
results = model('path_to_image.jpg')

# Display results
results.show()
