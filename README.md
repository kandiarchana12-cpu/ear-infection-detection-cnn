# Deep Learning-Based Ear Infection Detection

**Repository name:** `ear-infection-detection-cnn`
**Programme:** MSc Data Analytics, Berlin School of Business and Innovation | **Date:** [02/2026]

## Summary
A convolutional neural network (CNN) that classifies otoscopic (ear-camera) images as infected or healthy, to support quicker and more consistent first diagnosis, especially where ENT specialists are scarce. The thesis also surveys healthcare professionals on how far they would trust and use such a tool.

## Problem
Ear infections such as otitis media are usually diagnosed by visual inspection, which depends on the clinician's experience and can be inconsistent. The project tests whether a deep learning model can support this step.

## Data
- **Images:** labelled otoscopic images of healthy ears and ears with infection. Source: [add dataset name/link].
- **Survey:** structured questionnaire, 34 healthcare professionals (trust, usability, acceptance of AI-assisted diagnosis).
- *The images are medical data and are not included in this repository.*

## Method
1. **Preprocessing (OpenCV, NumPy, TensorFlow):** resizing, contrast enhancement, normalisation; removal of blurred or unusable images.
2. **Augmentation:** horizontal flip, rotation, zoom, brightness changes to reduce overfitting.
3. **Model (TensorFlow/Keras):** CNN with transfer learning from pre-trained networks. [Name the exact model you used, e.g. ResNet / EfficientNet.]
4. **Training:** hyperparameter tuning (learning rate, batch size, epochs) on a validation set; training curves monitored.
5. **Evaluation:** accuracy, precision, recall, F1-score and ROC-AUC on a held-out test set.

## Results
| Metric | Score |
|---|---|
| Accuracy | 91.3% |
| Precision | 89.7% |
| Recall (sensitivity) | 92.5% |
| F1-score | 91.1% |

High recall matters most here because a missed infection delays treatment. Survey results: [add 1-2 key findings from your Chapter 4].

## Tools
Python, TensorFlow, Keras, OpenCV, NumPy, Pandas, Matplotlib

## Limitations
- Image quality varies between otoscopes, lighting and angles.
- Binary classification only (infected vs. healthy), not infection types.
- Small practitioner sample (n = 34).

## Repository contents
`/notebooks` (training and evaluation code) | `/results` (charts, confusion matrix, ROC curve) | `README.md`

## Author
Archana Kandi | [https://www.linkedin.com/in/archana-kandi-536b86348/]
