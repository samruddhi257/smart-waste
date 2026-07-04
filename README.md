# Smart Waste Segregation

## Overview

This project implements an image classification model for automated waste segregation using transfer learning. A pretrained VGG16 network is fine-tuned on the TrashNet dataset to classify waste into six categories: cardboard, glass, metal, paper, plastic, and trash.

## Features

* VGG16 transfer learning for waste classification
* Fine-tuning using data augmentation and learning rate scheduling
* Classification of six waste categories
* Custom image and webcam inference
* Performance evaluation using accuracy, precision, recall, F1-score, and confusion matrix

## Dataset

This project uses the TrashNet dataset, which contains approximately 2,500 labeled images across six waste categories:

* Cardboard
* Glass
* Metal
* Paper
* Plastic
* Trash

Dataset: https://github.com/garythung/trashnet

## Model Architecture

* Pretrained VGG16 (ImageNet weights)
* Fine-tuned final convolutional block
* Global Average Pooling layer
* Dense layer
* Dropout layer
* Softmax output layer

## Results

| Metric            |  Value |
| ----------------- | -----: |
| Test Accuracy     | 87.11% |
| Macro F1-Score    |   0.85 |
| Weighted F1-Score |   0.87 |

## Requirements

Install the required Python packages:

```bash
pip install tensorflow opencv-python numpy matplotlib scikit-learn
```

## Usage

1. Open the notebook in Google Colab.
2. Download and extract the TrashNet dataset.
3. Run the notebook cells sequentially.
4. Train the model.
5. Test the model using custom images or the webcam inference section.
