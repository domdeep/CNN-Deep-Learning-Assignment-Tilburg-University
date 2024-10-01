# CNN-Deep-Learning-Assignment-Tilburg-University

# Brain Tumor Classification Using CNN

This project is part of the Deep Learning course (880008-M-6), at Tilburg University, Fall 2024. The goal of this assignment is to classify brain tumors using MRI images and Convolutional Neural Networks (CNNs). This repository includes the code files in Jupyter format and the report with discussions. 

## Overview

The project focuses on classifying different types of brain tumors (glioma, meningioma, pituitary tumors, and no tumor) using CNN architectures. Various techniques were applied, including hyperparameter tuning and transfer learning, to improve model performance. 

## Dataset

The dataset used for this project is the **Brain Tumor MRI Dataset**, available on Kaggle. It contains MRI images of four classes:
- Glioma
- Meningioma
- Pituitary
- No Tumor

The images were downscaled to 30x30 pixels due to computational constraints. The dataset is split into training, validation, and test sets.

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset).

## Models

### Baseline Model
- CNN with 32 filters per layer.
- ReLU activation functions with max pooling layers.

### Enhanced Model
- Additional convolutional and dense layers.
- Doubling the filters per layer.
- Implemented batch normalization and zero-padding.
- Early stopping based on validation loss.

### Transfer Learning
- Pre-trained architectures: VGG16, ResNet50, and DenseNet121.
- Grayscale images converted to RGB format for compatibility.
- Results were suboptimal for certain classes, especially meningioma, but improved with trainable layers.

