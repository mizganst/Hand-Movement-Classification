# Hand Movement Classification using HANDMI4 Glove Data
This project implements a machine learning pipeline to classify hand movements and mobility using motion tracking data. Specifically, it utilises wearable sensor data (glove-based) from the HANDMI4 dataset to compare different classification algorithms and feature reduction techniques.

# Project Overview
The study focuses on motion tracking data from 20 healthy subjects. While the original dataset includes both wearable IMU and camera-based systems, this analysis focuses exclusively on glove data. The pipeline includes data preprocessing, time-domain and frequency-domain feature extraction, and a comparative analysis of three popular classification models.

# Key Results
Best Model: Random Forest achieved the highest classification accuracy of 89.22%.

Optimisation: Applying Random Forest feature importance for feature reduction increased the model's accuracy by an additional 2%.

# Dataset
Source: HANDMI4 dataset (Mongelli & Menolotto, 2023).

Subjects: 20 healthy subjects.

Data Type: Wearable IMU glove data (CSV format) including accelerometer readings for various finger segments (e.g., Index_Prox_Acc_X) and joint angles (e.g., MCP_FE_Thumb, Wrist_FE).

# Methodology
1. Feature Extraction
The project extracts two types of features from the raw sensor data:

Time-Domain Features: Mean, maximum values, and standard deviation.

Frequency-Domain Features: Various frequency-based characteristics extracted before dataset splitting.

2. Model Training & Testing
The feature-extracted dataset is split into 80% for training and 20% for testing. Three classification algorithms were implemented and compared:

Random Forest (RF)

Support Vector Machine (SVM)

K-Nearest Neighbours (KNN)

3. Feature Reduction
To optimise performance, two techniques were evaluated:

Principal Component Analysis (PCA): Found to reduce overall accuracy in this specific implementation.

Random Forest Feature Importance: Successfully boosted accuracy by 2%.

# Getting Started
# Prerequisites
To run the notebook, you will need the following Python libraries:
To run the notebook, you will need the following Python libraries:

- pandas
- numpy
- scikit-learn
- matplotlib (for visualisations)

