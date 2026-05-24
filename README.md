# Intel Image Classification

Deep learning project for classifying Intel images into 6 categories using PyTorch CNN.

## Dataset

Images organized in train/test splits:
- Buildings
- Forest
- Glacier
- Mountain
- Sea
- Street

## Model Architecture

Convolutional Neural Network with:
- 2 convolutional blocks (Conv2d → ReLU → MaxPool2d)
- Fully connected classifier layer
- Input: 150×150 RGB images
- Output: 6 class predictions

## Training Setup

- **Loss Function**: CrossEntropyLoss
- **Optimizer**: Adam (lr=0.001)
- **Epochs**: 15
- **Batch Size**: 32
- **Device**: Auto GPU/CPU

## Data Augmentation

- Random horizontal flip (30% probability)
- Color jittering (brightness ±0.1, contrast ±0.2)
- ImageNet normalization

## Requirements

```
torch
torchvision
torchmetrics
torchinfo
```

## Usage

Run `Intel-Image-Classification.ipynb` to train and evaluate the model.
