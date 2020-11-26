---
layout: default
title: Preparation
parent: Computer Vision
nav_order: 2
permalink: /computer-vision/preparation
---

# Preparation

## Understand how your data is structured


Datasets are commonly shared in the following ways

1. Individual files representing images organised into folders or with filenames representing information about those items

2. A table of data such as a CSV in which each row is an item and may include filenames providing connections between the data in the table and the data in other formats such as images

**You can understand how the data is organised with the ```path.ls()``` method provided by fastai.**

It returns a special fastai L class which returns the # of items and the first 10 items in the path.

## Loss function

We choose a loss function to help train our model. The loss function gives us a sense of the accuracy of the model's performance for a set of parameters. It does this by comparing our models activations with the targets (labels) in the training dataset. 

The type of problem you are trying to solve will determine the type of loss function you end up using.

### Cross Entropy Loss
