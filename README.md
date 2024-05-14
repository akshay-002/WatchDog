<div align="center">
  <h1>Watchdog</h1>
</div>

## Introduction

This repository contains the code for a Driver Drowsiness Detection system using Convolutional Neural Networks (CNN) with Python and OpenCV, aiming to reduce road accidents by alerting drowsy drivers with an alarm. The system detects faces in images and categorizes them as either yawning or non-yawning, as well as whether the eyes are open or closed. It utilizes Haar cascade classifiers for face and eye detection, and a trained CNN model for classification.


A CNN, trained to distinguish between open and closed eyes, processes live video feed from a camera. Each frame is analyzed by the CNN, and if the eyes remain closed for three seconds, the system triggers an alert to ensure driver safety.

## Contents

- [Watchdog](#watchdog)
  - [Introduction](#introduction)
  - [Contents](#contents)
  - [Jupyter Notebook: Driver Drowsiness Detector - CNN](#jupyter-notebook-driver-drowsiness-detector---cnn)
  - [Python File: Real-time Drowsiness Detection](#python-file-real-time-drowsiness-detection)
  - [The Output : Real-time Detection Screenshorts](#python-file-real-time-drowsiness-detection)

## Jupyter Notebook: Driver Drowsiness Detector - CNN

### Table of Contents:

1. [Data Exploration](#1-data-exploration)
2. [Data Preprocessing](#2-data-preprocessing)
3. [Data Augmentation](#4-data-augmentation)
4. [Model Architecture and Training](#4-model-architecture)
5. [Evaluating Model Performances](#5-evaluating-model-performances)
6. [Predictions](#7-predictions)
7. [Conclusion](#8-conclusion)
8. [Acknowledgements](#9-thankyou)

The Jupyter notebook file (`driver_drowsiness.ipynb`) contains the complete pipeline for the driver drowsiness detection system. It includes data exploration, preprocessing, model training, evaluation, and predictions. Various techniques such as data augmentation and CNN architecture design are discussed.

## Python File: Real-time Drowsiness Detection

The Python file (`real_time_drowsiness_detection.py`) implements real-time drowsiness detection using the trained CNN model. It utilizes OpenCV for capturing video frames, Haar cascade classifiers for face and eye detection, and TensorFlow/Keras for model inference. When drowsiness is detected, an alarm sound is played to alert the driver.

Both files use the trained model (`Watchdog.h5`) for drowsiness detection. The model achieved an accuracy of 96% during training.

## System Overview

This system is designed to detect driver drowsiness using a combination of CNN, Python, and OpenCV. The primary goal is to reduce road accidents by alerting drivers when they show signs of drowsiness.

## The Output 

1. Open Eyes:
   ![Drowsiness Dataset](Images/Eyes_open.png)
   

3. Close eyes
   Here we detect wheater the eyes are closed and count the number of frames for which the eyes were closed (which is 10 frame) greater then that the Alarm will ring and the WARNING sign is displayed.
   ![Drowsiness Dataset](Images/Eyes_closed.png)

   
Feel free to explore the code and adapt it to your specific requirements. If you have any questions or suggestions, please don't hesitate to reach out!

---

*Note: Make sure to install all required dependencies and ensure proper file paths before running the code.*
