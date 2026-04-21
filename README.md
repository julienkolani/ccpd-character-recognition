# CCPD Character Recognition

License plate character recognition pipeline using the Chinese City Parking Dataset (CCPD). Achieves 81.47% accuracy on alphanumeric classification without deep learning.

## Overview

Implements a profile-matching approach: distance-to-edge feature extraction combined with K-means clustering for template learning. Characters (0-9, A-Z) are classified using Euclidean distance to cluster centroids with softmax probability conversion.

## Results

- Dataset: CCPD (Chinese Province City District license plates)
- Test set: ~475 images
- Accuracy: **81.47%** on alphanumeric characters (0-9, A-Z)

## Tech Stack

- Python
- OpenCV
- NumPy
- scikit-learn (K-means, confusion matrix)
- Matplotlib

## Setup

```bash
pip install opencv-python numpy scikit-learn matplotlib
jupyter notebook
```

## Dataset

The CCPD dataset is not included. Download it separately and place it in `data/`.
