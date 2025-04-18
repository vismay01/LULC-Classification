# EuroSAT LULC Classification using ResNet

## Overview

This project implements Land Use and Land Cover (LULC) classification on the EuroSAT dataset using ResNet deep learning architecture. The model classifies satellite images into 10 different land use categories with high accuracy.

## Dataset

The [EuroSAT dataset](https://github.com/phelber/EuroSAT) contains 27,000 labeled Sentinel-2 satellite images (64×64 pixels) covering 13 spectral bands and consisting of 10 classes:

- Annual Crop
- Forest
- Herbaceous Vegetation
- Highway
- Industrial
- Pasture
- Permanent Crop
- Residential
- River
- Sea & Lake

## Model Architecture

This implementation uses ResNet (Residual Neural Network), specifically ResNet-50, which is well-suited for image classification tasks. The architecture includes:

- Pre-trained weights from ImageNet (with transfer learning)
- Custom final classification layer for the 10 EuroSAT classes
- Residual connections to mitigate the vanishing gradient problem


## Model Performance

| Model     | Accuracy | F1-Score |
|-----------|----------|----------|
| ResNet-50 | 95.7%    | 0.956    |
