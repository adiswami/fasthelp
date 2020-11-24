---
layout: default
title: Data Augmentation
parent: Computer Vision
nav_order: 2
permalink: /docs/computer-vision/data-augmentation
---

# Data Augmentation

## Presizing

A unique approach to data augmentation provided by the fastai library designed to minimize data destruction and maintain performance.  
Presizing involves two steps and is used when constructing a DataBlock.

1. Resize images to relatively "large" dimensions; ie. larger than the target training dimensions. This is done to each individual image and on the CPU.
```
#Increase the image size to 460x460
item_tfms=Resize(460)
```

2. Compose all the common augmentation operations into one, including the resize to the final target size. This is done on the GPU as a batch.
```
#Common data augmentation bundled into the aug_transforms method
#RandomResizedCrop is added when min_scale is called, crop size 224x224 which is a common target size for training
batch_tfms=aug_transforms(size=224, min_scale=0.75)
```
