### Satellite Image Segmentation with U-Net++
This repository contains a complete pipeline for semantic segmentation of satellite imagery using multispectral (MSI) and synthetic aperture radar (SAR) data. The project leverages U-Net++ with a ResNeSt encoder to classify land cover into 14 distinct classes, including water, streets, vegetation, and urban areas.

### Features
Data Handling: Includes utilities for downloading, extracting, and visualizing MSI and SAR images with labeled ground truth.
Custom Dataset Class: Efficient data preprocessing and augmentation using albumentations.
Deep Learning Model: Implements U-Net++ with 6 input channels for MSI + SAR data.
Training Pipeline: Tracks loss, validation IoU, and saves the best-performing model.
Metrics: Computes class-wise and mean IoU, F1 Score, Precision, and Recall using torchmetrics.
Visualization: Compares true labels with predicted outputs for qualitative assessment.
### Technologies Used
PyTorch: Core framework for model training and dataset handling.
segmentation_models_pytorch: Provides U-Net++ architecture with pretrained encoders.
albumentations: Data augmentation and preprocessing.
GDAL: Handles geospatial raster data.
matplotlib: Visualizes results and performance metrics.
### Getting Started
Data: The script automatically downloads and extracts the dataset.
Dependencies: Install the required Python libraries (torch, segmentation_models_pytorch, albumentations, etc.).
Training: Customize training settings and start training using the provided script.
Evaluation: Evaluate the model on test data with detailed performance metrics and visualizations.
### Applications
Land cover classification
Environmental monitoring
Urban planning and infrastructure analysis
### Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to enhance functionality.
