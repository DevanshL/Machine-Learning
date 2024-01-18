# Convolutional Neural Network (CNN) 

## Overview

This project involves the implementation of a Convolutional Neural Network (CNN) for a specific purpose. 

## Data Preprocessing
 Data preprocessing is crucial for training an effective CNN model. In this project, the following steps are performed using TensorFlow's ImageDataGenerator:

* Normalization: Pixel values are rescaled to the range [0, 1].
* Shear, Zoom, and Horizontal Flip Augmentation: Enhances the variety of training data.
* Flow from Directory: Reads and preprocesses images directly from the specified directories.

## Model Architecture
The CNN model architecture consists of the following key steps:

* `Convolution (Step 1)`: The initial layer applies convolution with 32 filters, a kernel size of 3x3, and ReLU activation. The input shape is set to [64, 64, 3].

* `Pooling (Step 2)`: Max pooling is applied with a pool size of 2x2 and a stride of 2 to downsample the feature maps.

* `Flattening`: Flattens the output to a one-dimensional array, preparing it for the fully connected layers.

* `Full Connection`: Two dense layers are added with 128 units and ReLU activation, followed by an output layer with a sigmoid activation for binary classification.

## Training
  The CNN is trained on the provided training set. The training process involves multiple epochs, where the model learns to map input images to their corresponding binary classes.

## Evaluation
  The trained CNN is evaluated on the test set to assess its performance. The evaluation includes computing metrics such as accuracy and loss.  

## Making Predictions
  The trained CNN can be used to make predictions on new images. A single prediction example is provided using the model.
