# Pothole Detection System  

A machine learning-based system designed to detect potholes on roads using advanced image processing techniques.  

## Table of Contents  

- [Introduction](#introduction)  
- [Features](#features)  
- [Dataset](#dataset)  
- [Model Architecture](#model-architecture)  
- [Installation](#installation)   
- [Demo Video](#demo-video)


## Result Image
<img width="959" alt="Result" src="https://github.com/user-attachments/assets/01bd8dd7-849e-465e-8707-8787b0178527" />

## Result Video
[Road Damage Assessment](https://github.com/drashti-03/pothole-detection-system/releases/tag/pothole-detection)  


## Introduction  

Potholes pose a serious risk to road safety and vehicle maintenance. This project aims to develop a deep learning-based pothole detection system that can analyze images or videos of roads and identify potholes, enabling timely repairs and improved road conditions.  

## Features  

✅ **Real-time Detection** – Works with both images and video streams.  
✅ **High Accuracy** – Trained using Convolutional Neural Networks (CNNs).  
✅ **Easy Integration** – Can be deployed in real-world applications like traffic monitoring systems.  

## Dataset  

Pothole_Segmentation_YOLOv8 - v1 2023-10-20 10:09pm
==============================

This dataset was exported via roboflow.com on January 26, 2024 at 9:04 AM GMT

Roboflow is an end-to-end computer vision platform that helps you
* collaborate with your team on computer vision projects
* collect & organize images
* understand and search unstructured image data
* annotate, and create datasets
* export, train, and deploy computer vision models
* use active learning to improve your dataset over time

For state of the art Computer Vision training notebooks you can use with this dataset,
visit https://github.com/roboflow/notebooks

To find over 100k other datasets and pre-trained models, visit https://universe.roboflow.com

The dataset includes 780 images.
Pothole are annotated in Tensorflow Object Detection format.

The following pre-processing was applied to each image:
* Auto-orientation of pixel data (with EXIF-orientation stripping)
* Resize to 640x640 (Stretch)

The following augmentation was applied to create 3 versions of each source image:
* 50% probability of horizontal flip
* Randomly crop between 0 and 20 percent of the image
* Random rotation of between -15 and +15 degrees
* Random shear of between -5° to +5° horizontally and -5° to +5° vertically
* Random brigthness adjustment of between -25 and +25 percent
* Random exposure adjustment of between -25 and +25 percent 

## Model Architecture  

The pothole detection system is built using **YOLOv8**, a state-of-the-art object detection model. The model is trained with the following parameters:  

- **Base Model**: YOLOv8  
- **Training Epochs**: 50  
- **Image Size**: 640x640 pixels  
- **Batch Size**: 16  
- **Early Stopping Patience**: 10 epochs  
- **Optimizer**: Auto (chooses the best from [SGD, Adam, Adamax, AdamW, NAdam, RAdam, RMSProp])  
- **Initial Learning Rate**: 0.0001  
- **Final Learning Rate**: 0.01 (calculated as `lr0 * lrf`)  
- **Dropout Regularization**: 25%  
- **Device**: CUDA (GPU) – `device=0`  
- **Random Seed**: 42 (for reproducibility)  

The model has been fine-tuned for robustness across various road conditions.    

