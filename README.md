# Object-Detection
This project evaluates the YOLOv8 object detection model for identifying roadside objects to enhance autonomous driving safety. Fine-tuning a YOLOv8s model with a custom dataset enabled effective detection of vehicles, pedestrians, and traffic signs under div.erse conditions
# Road Condition Detection Using YOLOv8

## Project Overview
This project investigates the effectiveness of the YOLOv8 object detection model for detecting roadside objects, enhancing safety and situational awareness in autonomous driving systems. YOLOv8's balance between speed and accuracy makes it a strong candidate for real-time applications. The model was fine-tuned using a custom dataset to recognize objects like vehicles, pedestrians, and traffic signs under diverse environmental conditions.

## Abstract
The project utilizes YOLOv8s (small variant) to detect roadside objects accurately, ensuring real-time performance. Extensive hyperparameter tuning and dataset augmentation were applied to optimize the model's detection capabilities, achieving high accuracy and robustness, even in challenging scenarios. Results demonstrated competitive Mean Average Precision (mAP) scores, minimal false positives, and reliable detection across complex road environments.

## Literature Review
- Traditional approaches like sliding windows and R-CNN struggled with real-time processing.
- Advances in deep learning and CNNs led to the development of models like YOLO, which prioritize speed and efficiency.
- YOLOv8 builds upon previous iterations, incorporating advanced techniques like attention mechanisms and improved convolutional layers, making it ideal for real-time object detection tasks.

## Dataset
- **Name**: Project Road.v4i (Custom)
- **Content**: Labeled images of roadside objects (vehicles, traffic signs, pedestrians) in diverse lighting and environmental conditions.
- **Annotations**: YOLO format for bounding boxes and class labels.
- **Structure**: Split into training, validation, and test sets to ensure robust evaluation.

## Methodology
1. **Model**: YOLOv8s with pre-trained weights.
2. **Hyperparameters**:
   - Learning rate: 0.01 (decayed to stabilize training).
   - Batch size: 16.
   - Image size: 224x224 pixels.
   - Training epochs: 50.
3. **Evaluation Metrics**:
   - Mean Average Precision (mAP).
   - Precision-Recall curves.
   - Confusion matrices for classification performance.

## Results
- Achieved high mAP scores across multiple classes.
- Demonstrated strong performance in challenging conditions (e.g., low light, cluttered backgrounds).
- Visual analysis confirmed effective detection with minimal false positives.

## Future Work
- Expand the dataset to include rarer objects and more complex scenarios.
- Experiment with YOLOv8 variants (e.g., YOLOv8m, YOLOv8l) for enhanced accuracy.
- Optimize the model for deployment in edge computing or hardware-accelerated environments.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/road-condition-detection.git
