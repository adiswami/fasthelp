---
layout: default
title: Data Exploration
parent: Computer Vision
nav_order: 1
permalink: /computer-vision/data-exploration
---

# Data Exploration

## Check DataBlock

Once you have created your ```DataBlock```, make sure it looks ok with the ```show_batch``` method: 

```
#Shows a sample of data
dls.show_batch(nrows=1, ncols=3)
```
