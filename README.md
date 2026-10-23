# Mango Leaf Disease Diagnosis using CNN

## Overview
This project uses a Convolutional Neural Network (CNN) to classify mango leaf images into eight categories using the MangoLeafBD dataset.

## Dataset
- **Source:** [MangoLeafBD — Mendeley Data](https://data.mendeley.com/datasets/hxsnvwty3r/1)
- **Total images:** 4,000
- **Classes:** Anthracnose, Bacterial Canker, Cutting Weevil, Die Back, Gall Midge, Healthy, Powdery Mildew, Sooty Mould.

## Methodology
- Image resizing to 160 × 160 pixels and pixel normalization.
- Data augmentation using horizontal flipping, rotation, and zoom.
- CNN with three convolutional layers, max pooling, global average pooling, and dropout.
- Adam optimizer and sparse categorical cross-entropy loss.
- Perceptual-hash grouping to reduce near-duplicate leakage between data splits.

## Results
- **Test accuracy:** 70.02%
- **Test macro F1-score:** 0.7038
- **Test images:** 577

## Files
- `RA2311026050007_PS03.ipynb` — Notebook containing preprocessing, training, and evaluation.
- `PS03_MangoLeaf_CNN.keras` — Trained CNN model.

## Limitations
The dataset contains visually similar and transformed copies of some leaves. Perceptual hashing helps reduce overlap between splits but may not detect every near-duplicate. Further training and validation on independently collected field images are needed.

## Tools and Technologies
Python, TensorFlow/Keras, NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn.

## Note
This project is for educational purposes. The model is not a substitute for expert plant disease diagnosis.
