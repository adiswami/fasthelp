---
layout: default
title: Verification
parent: Computer Vision
nav_order: 4
permalink: /computer-vision/verification
---

# Verification

## Check DataBlock

Once you have created your ```DataBlock```, make sure it looks ok with the ```show_batch``` method: 

```
#Shows a sample of data
dls.show_batch(nrows=1, ncols=3)
```
