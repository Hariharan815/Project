**Plant Species Prediction Using Deep Learning**
**Project Overview**
This project is a Plant Species Classification System built using Deep Learning and Transfer Learning. It uses the MobileNetV2 pre-trained CNN model to classify plant species from images. The system helps in automatic plant identification with high accuracy and efficient training performance.

**Features**
Image-based plant species classification
Transfer Learning using MobileNetV2
Data augmentation for better generalization
Automatic class label detection
Real-time image prediction support

**Model Architecture**
Base Model: MobileNetV2 (ImageNet Pretrained)
Custom Layers Added:
Global Average Pooling
Dense (1024 neurons, ReLU)
Output Dense Layer (Softmax)
Loss Function: Categorical Crossentropy
Optimizer: Adam

**Technologies Used**
Python
TensorFlow / Keras
MobileNetV2
NumPy
Matplotlib
Google Colab

**Dataset Structure**
Dataset should be organized as:
plants prediction/
│
├── Rose/
├── Sunflower/
├── Tulip/
├── Daisy/
└── Other_Plant_Species/
Dataset loaded from compressed .rar file and extracted programmatically.

**Data Preprocessing**
Image Rescaling (1./255)
Rotation Augmentation
Zoom Augmentation
Horizontal Flip
Validation Split: 20%

**Model Training**
Input Image Size: 224 × 224
Batch Size: 32
Epochs: 10

Training Strategy:
Base MobileNetV2 layers frozen
Only custom layers trained initially

**Model performance**
**Metric	Value**
Validation Accuracy	90% – 93%
Validation Loss	0.25 – 0.40
