# Blood Cells Classification

## Overview

This project was developed for the course *Artificial Neural Networks and Deep Learning* (AN2DL) at Politecnico di Milano (A.Y. 2024-2025). The goal was to classify blood cell images into 8 different categories using Convolutional Neural Networks (CNNs), applying both custom architectures and transfer learning.

The dataset consists of 13,759 RGB images of size 96x96, labeled as:
- Basophil
- Eosinophil
- Erythroblast
- Immature Granulocytes
- Lymphocyte
- Monocyte
- Neutrophil
- Platelet

After cleaning duplicated and mislabeled images, the final dataset contains 11,943 images.

## Project Highlights

- **Data Cleaning**: Duplicated and altered images were removed.
- **Custom CNNs**: Two models were tested (a shallow CNN and a VGG-inspired one), but suffered from overfitting.
- **Transfer Learning**: MobileNetV3 and EfficientNetB0 were used as pre-trained feature extractors.
- **Fine-Tuning**: Selective unfreezing of EfficientNetB0 layers improved performance.
- **Augmentation**: RandAugment was applied offline to improve generalization.
- **Optimizer Tuning**: Adam with learning rate 0.0001 proved optimal.
- **Final Accuracy**: Validation accuracy ~98.7%, Codabench accuracy ~77.0%.

## Files in the Repository

- `Notebooks/`: Jupyter notebooks containing code for model training, augmentation, and evaluation.
- `Report.pdf`: Complete report with analysis, models, methodology, and results.

> ⚠️ **Note**: The dataset is not included due to size and license constraints.

## Authors

Camilla Bocciolone, Davide Fileccia, Luca Forte, Matilde Simonetti  


