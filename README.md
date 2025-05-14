# ViT-DeepLabv3 for ADE20K Semantic Segmentation

This repository contains the implementation of a hybrid semantic segmentation architecture that combines Vision Transformer (ViT) with DeepLabv3 for the ADE20K dataset.

## Overview

Our approach leverages transfer learning by using a pretrained DeepLabv3 model with a ResNet101 backbone, adapting it to the 151-class ADE20K semantic segmentation task. Through fine-tuning, we achieve a significant improvement in mean IoU from 0.2189 to 0.4954.

## Dataset

This implementation uses the ADE20K dataset:
- 150 semantic categories + background class (151 total)
- ~20,000 training images and 2,000 validation images
- Complex scenes with multiple overlapping objects

The dataset should be organized in the following structure:
```
./data/ADE20K/
├── images/
│   ├── training/
│   └── validation/
└── annotations/
    ├── training/
    └── validation/
```

You can download the dataset from the [MIT Scene Parsing Benchmark website](http://sceneparsing.csail.mit.edu/).

## Getting Started

To run this code, please use the Colab notebook provided in the following link:

[Open in Google Colab](https://colab.research.google.com/drive/1yi3vMYpM_AG3kBENx6wLL8hCYPIKciO8?usp=sharing)

The Colab notebook contains all necessary code, setup instructions, and examples.

## Performance

Our model achieves 49.54% mean IoU on the ADE20K validation set, representing a 126.3% improvement over the initial transfer model of 21.89% IoU.

