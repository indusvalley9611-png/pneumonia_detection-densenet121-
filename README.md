
# Pneumonia Detection Using DenseNet121

## Overview
This project explores binary pneumonia classification from chest X-ray images using transfer learning with DenseNet121 and TensorFlow/Keras. It includes model evaluation, classification threshold analysis, and Grad-CAM visualization to inspect image regions influencing model predictions.

## Features
- Chest X-ray preprocessing
- DenseNet121 transfer learning
- Binary pneumonia classification
- Precision, recall, specificity, F1-score, and confusion matrix
- Precision–Recall curve and Average Precision
- Grad-CAM heatmaps and overlays
- Interactive image upload for model experimentation

## Technology Stack
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- scikit-learn
- Pillow
- pydicom
- OpenCV
- ipywidgets
- Jupyter Notebook / Kaggle

## Dataset
RSNA Pneumonia Detection Challenge:
https://www.kaggle.com/c/rsna-pneumonia-detection-challenge/data

Download the dataset through Kaggle and configure the notebook paths for your environment. Do not commit the dataset to this repository.

## Model Evaluation
Validation results from one experiment:

| Metric | Result |
|---|---:|
| Validation accuracy | Approximately 80% |
| Average Precision | 0.6366 |
| Precision | 0.5360 |
| Recall | 0.7180 |
| Specificity | 0.8193 |
| F1-score | 0.6138 |
| Selected threshold | 0.6370 |

These metrics were obtained on a validation set of 5,337 images. Results depend on the model checkpoint, preprocessing, and threshold. They are experimental and are not evidence of clinical diagnostic performance.

## Run the Project
1. Clone this repository.
2. Install dependencies from `requirements.txt`.
3. Download the dataset from Kaggle.
4. Open `pneumonia_detection.ipynb` in Jupyter or upload it to Kaggle.
5. Update dataset paths and run the notebook cells in order.

## Grad-CAM
Grad-CAM generates a heatmap and overlay to help inspect regions influencing model output. Highlighted regions do not prove the presence of pneumonia.

## Limitations
- Performance may vary across datasets and imaging equipment.
- Input preprocessing must match the training pipeline.
- Predictions require independent evaluation and clinical validation before any medical use.

## Disclaimer
This is an educational machine learning project, not a medical diagnostic tool.
