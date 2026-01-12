# Workout-video-classifier
This repository contains a deep learning project for classifying workout exercise videos using a pretrained **3D CNN (ResNet R3D-18)**.

### Project Overview
* Task: Multi-class classification of workout videos
* Dataset: ~650 short videos across 22 exercise classes (imbalanced)

### Model
* Backbone: **ResNet R3D-18** pretrained on Kinetics
* Fine-tuning: Layers 3, 4, and fully connected layer
* Loss: Weighted Cross-Entropy
* Optimizer: Adam
* Regularization: Early stopping, weighted sampling, data augmentation

### Preprocessing
* Uniform frame sampling
* Frame resizing to 112×112
* Spatial augmentations (train only)
* Normalization using pretrained model statistics

### Results
* Train Accuracy: ~99%
* Validation Accuracy: ~97%
* Test Accuracy: ~95%
* Strong generalization despite small and imbalanced dataset

