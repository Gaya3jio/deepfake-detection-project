# deepfake-detection-project
# Deepfake Video Detection using CNN and MobileNetV2

This project is a deep learning-based system that detects deepfake videos by analyzing extracted frames using both a custom Convolutional Neural Network (CNN) and a pretrained MobileNetV2 model.

## Overview

- Detects manipulated (fake) video frames vs. real ones.
- Built using TensorFlow, Keras, and OpenCV.
- Achieved ~82% accuracy using MobileNetV2, ~81% with CNN.

## Models Used

- **Custom CNN**: Built from scratch using Conv2D, MaxPooling, Dense layers.
- **MobileNetV2**: Transfer learning with a custom classification head.
- Loss Function: Binary Crossentropy  
- Optimizer: Adam  
- Input: 30 frames per video, resized to 224×224


##  Results

| Model         | Accuracy |
|---------------|----------|
| CNN           | ~81%     |
| MobileNetV2   | ~82%     |

Confusion matrices and classification reports were used to evaluate performance. The models performed better at detecting fake frames, with future work needed to improve real-frame classification.

##  Requirements

- Python 3.x  
- TensorFlow  
- Keras  
- OpenCV  
- NumPy  
- Matplotlib  
- Scikit-learn  

Install them with:

```bash
pip install -r requirements.txt


