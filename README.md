# Histopathologic Cancer Detection

This project focuses on binary classification of histopathologic images to detect metastatic cancer. The task involves identifying whether small 96x96 pixel patches from histopathology slides contain cancerous tissue.

## Overview
- **Challenge**: Classify images as `0` (no cancer) or `1` (cancer) using deep learning.
- **Dataset**: [Kaggle Histopathologic Cancer Detection](https://www.kaggle.com/c/histopathologic-cancer-detection).
- **Approach**:
  1. Baseline model with `MobileNetV2` (pretrained, frozen base layers).
  2. Improved model with fine-tuning and dropout regularization.

## Key Results
- **Baseline Model**:
  - Validation Accuracy: ~84.88%
  - Validation Loss: ~0.3430
- **Improved Model**:
  - Validation Accuracy: ~89.98%
  - Validation Loss: ~0.2488

## Steps
1. **Exploratory Data Analysis (EDA)**:
   - Visualized label distribution and sample images.
2. **Model Development**:
   - Baseline: Pretrained `MobileNetV2` with frozen layers.
   - Improved: Fine-tuned the last 20 layers and added dropout for regularization.
3. **Training**:
   - Used data augmentation and early stopping.
   - Trained for 5 epochs due to computational constraints.
4. **Evaluation**:
   - Compared validation metrics between baseline and improved models.
5. **Submission**:
   - Generated predictions for test set and prepared Kaggle submission.
  
Kaggle Scores:
Private Score 0.7941
Public Score 0.8424
