# -Kannada-Digit-Recognition-PS41
CNN-based Kannada handwritten digit recognition with domain-shift analysis using Dig-MNIST

**Student:** Rokith S  
**Register Number:** RA2311026050045  
**Problem Statement:** PS-41  

## Objective
Classify handwritten Kannada digits (0–9) using a Convolutional Neural Network (CNN). Evaluate the model on the standard Kannada-MNIST test set and Dig-MNIST to analyze domain shift.

## Dataset
- Kannada-MNIST training set: 60,000 images
- Kannada-MNIST standard test set: 10,000 images
- Dig-MNIST external test set: 10,240 images
- Classes: 10 Kannada digits (0–9)

## Model
A CNN with three convolution blocks, batch normalization, max pooling, dropout, and dense layers was trained using TensorFlow/Keras.

## Results

| Dataset | Accuracy | Loss |
|---|---:|---:|
| Kannada-MNIST standard test set | 97.27% | 0.1000 |
| Dig-MNIST external test set | 78.35% | 1.2102 |

**Accuracy drop:** 18.92 percentage points.

## Domain Shift Analysis
The model performed strongly on the in-domain Kannada-MNIST test set but showed lower accuracy on Dig-MNIST. The drop occurs because Dig-MNIST contains handwriting from different volunteers and different image-collection conditions, leading to differences in stroke style, shape, thickness, alignment, noise, and image quality.

## Repository Contents
- `RA2311026050045_PS41.ipynb` — completed Colab notebook with outputs
- `final_results.csv` — accuracy and loss results
- PNG files — sample images, confusion matrices, accuracy comparison, and incorrect predictions
