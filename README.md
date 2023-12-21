# Landslide-Detection-with-Multi-Spectral-Satellite-Imagery-and-Image-Segmentation

This is my senior year phase-1 project involving the use of landslide-correlated features such as NDVI, DEM, Slope scores, and RGB images to train image segmentation models. The goal is to enhance the performance of landslide detection and mitigate disasters.

## Key Features

### UNet:
- Symmetric encoder-decoder architecture for pixel-wise image segmentation.
- Utilizes skip connections to capture both local and global context, enhancing segmentation accuracy.
- Employs a sigmoid activation function in the final layer for pixel-wise probability predictions.
- Trained using binary cross-entropy loss function designed for pixel-wise binary classification.

### FCN:
- Specialized deep learning architecture for pixel-wise image segmentation.
- Lacks fully connected layers, allowing handling of images with varying sizes.
- Relies on convolutional layers, contraction and extraction techniques to provide dense pixel-level predictions.
- Uses a sigmoid activation function in the final layer and binary-cross entropy loss function for training.

## Proposed Model Architecture
![image](https://github.com/suryapraneeth18/Landslide-Detection-with-Multi-Spectral-Satellite-Imagery-and-Image-Segmentation/assets/75241973/0dfec585-b3d7-47f1-a4a7-5cbf2056dc08)

## Results

**Validation Data**

- **UNet:**
  - Precision: 0.77
  - Recall: 0.68
  - F1 Score: 0.72

- **FCN:**
  - Precision: 0.77
  - Recall: 0.64
  - F1 Score: 0.70

**Test Data**

- **UNet:**
  - Precision: 0.78
  - Recall: 0.68
  - F1 Score: 0.72

- **FCN:**
  - Precision: 0.73
  - Recall: 0.64
  - F1 Score: 0.68

## Predictions

![image](https://github.com/suryapraneeth18/Landslide-Detection-with-Multi-Spectral-Satellite-Imagery-and-Image-Segmentation/assets/75241973/c3989d46-d2c3-412c-8c0d-0c87caa36c39)

Visualization of input bands, ground truth, and predictions: 
(a) RGB, (b) NDVI, (c) Slope, (d) DEM, (e) Ground Truth, (f) UNet Prediction, (g) Customized FCN Prediction.
