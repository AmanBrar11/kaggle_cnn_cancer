# Cancer Detection from Pathology Scans

## Overview

This project aims to develop a Convolutional Neural Network (CNN) capable of identifying the presence of cancer in pathology scan images. Such models hold significant potential in assisting medical professionals by facilitating early detection and treatment of serious diseases like cancer. This project uses data from the [Histopathologic Cancer Detection Kaggle Competition](https://www.kaggle.com/c/histopathologic-cancer-detection/overview)

## Data

The dataset comprises 220,025 training images and 57,458 test images, all in ".tif" format. The labels for these images, indicating the presence (1) or absence (0) of malignant cells, are provided in accompanying ".csv" files.

## Approach

The project involves several key steps:
1. **Exploratory Data Analysis (EDA):** Initial analysis revealed a 40.5% prevalence of positive (malignant) cases in the training set. Sample images were reviewed to understand the visual distinction between positive and negative cases.
2. **Data Preparation:** Utilized ImageDataGenerator for preprocessing and data augmentation to feed into the model.
3. **Model Architecture:** The model features three convolutional layers followed by max-pooling, a dense layer with dropout for regularization, and a sigmoid output layer for binary classification. Early stopping was employed to halt training when no significant improvement was observed, optimizing both the number of epochs and computational efficiency.

## Results

Despite experimenting with different architectures and parameters, the highest accuracy achieved was around 50%. While not highly accurate, incremental improvements were observed with certain adjustments like layer reduction and epoch modification. The chosen model balanced training efficiency and performance, considering the computational demands that sometimes extended training times up to 6 hours.

## Conclusion

The project serves as a proof of concept for using CNNs in medical image analysis, specifically cancer detection. While the current model's performance is modest, it highlights the potential for future improvements and the importance of such applications in healthcare.
