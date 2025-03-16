# Unsupervised Anomaly Detection in Industrial Inspection

## Project Overview
This project implements an **unsupervised anomaly detection system** for industrial inspection using **deep learning**. The model identifies defects in manufacturing products by analyzing images and detecting deviations from normal patterns.

## Features
- Uses **Anomalib**, a specialized library for anomaly detection.
- Implements **PatchCore**, a state-of-the-art anomaly detection model.
- Supports **MVTec AD**, an industrial anomaly detection dataset.
- Visualizes **anomaly heatmaps and masks** for better interpretability.
- Runs efficiently on **GPU (T4/P100) or TPU (v3-8)**.

## Dataset
- **MVTec AD**: A widely used benchmark dataset for anomaly detection.
- Categories: Bottles, Cables, Capsules, Metal Nuts, etc.
- Each category contains **normal and anomalous** images for training and evaluation.

## Installation
Ensure you have **Python 3.8+** and install the required dependencies:
```bash
pip install anomalib
pip install wandb
```

## Model & Methodology
- **PatchCore** is used due to its efficiency and high detection accuracy.
- **Anomaly heatmaps** highlight defective areas in the images.
- **Resizing and preprocessing** ensure compatibility with the model.

## Training & Inference
- **Training** is performed on normal images to learn the standard patterns.
- **Inference** is run on test images to classify and localize anomalies.
- **Visualization** helps interpret the results effectively.

## Results
- Generates **heatmaps and binary masks** for defect localization.
- Achieves high **precision and recall** on the MVTec AD dataset.
- Can be fine-tuned for **custom industrial datasets**.

## Troubleshooting
- **Black images in visualization?** Ensure proper image normalization.
- **ModuleNotFoundError?** Check if `anomalib` is correctly installed.
- **Dataset not found?** Verify the dataset path in your notebook.

## Future Work
- Implement **real-time anomaly detection**.
- Explore **self-supervised learning** for improved performance.
- Deploy the model for **industrial automation**.

## References
- [Anomalib Documentation](https://openvinotoolkit.github.io/anomalib/)
- [MVTec AD Dataset](https://www.mvtec.com/company/research/datasets/mvtec-ad/)

