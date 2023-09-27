<!-- # ImageSegmentation
Dataset COCO
Number of training images 1000
Base model fcn_resnet101
Number of classes to be segmented 3: 0 Background, 1 Person, 2 car -->

# Semantic Segmentation with FCN-ResNet101

This repository contains an implementation of semantic segmentation using a modified FCN-ResNet101 model trained on the COCO dataset. The model is capable of segmenting specific classes (e.g., 'person' and 'car') from images.

## Overview

- **Dataset**: The COCO dataset is used for training and testing the semantic segmentation model. A subset of images containing specific classes (e.g., 'person' and 'car') is selected for training.

- **Model**: The model architecture is based on FCN-ResNet101, a fully convolutional network with a ResNet101 backbone. The classifier head is modified to output the desired number of classes (including a background class).

- **Training**: The model is trained on the selected COCO dataset subset. Cross-entropy loss is used as the training objective. Training details and loss per epoch are recorded.

- **Inference**: After training, the model can be used for semantic segmentation on new images. An example image is provided for testing the model's inference capability.