# simple_cnn_model_keras_cifar10_dataset
# This repository contains the implementation of simple CNN Model using Keras on CIFAR-10 Dataset

## Basic of the CNN Architecture:
-> Convolution Neural Networks(CNN) are the deep feed-forward neural networks that is used for analysing the Images.
-> CNN is used for Classfaction of image, it outputs the probability of classes that best describe that image.

### CNN Layers:
There are 5 basic building bloacks of CNN Architecture. They are:
1. Convolution Layer
2. ReLu Layer
3. Pooling Layer
4. Fully-Connected Layer
5. Loss Layer

A simple ConvNet for CIFAR-10 classification could have the architecture [INPUT - CONV - RELU - POOL - FC]. In more detail:

INPUT [32x32x3] will hold the raw pixel values of the image, in this case an image of width 32, height 32, and with three color
channels R,G,B.CONV layer will compute the output of neurons that are connected to local regions in the input, each computing a
dot product between their weights and a small region they are connected to in the input volume. This may result in volume such as
[32x32x12] if we decided to use 12 filters.

CONV layer will compute the output of neurons that are connected to local regions in the input, each computing a dot product 
between their weights and a small region they are connected to in the input volume. This may result in volume such as 
[32x32x12] if we decided to use 12 filters.

RELU layer will apply an elementwise activation function, such as the max(0,x)thresholding at zero. This leaves the size of the volume unchanged ([32x32x12]).

POOL layer will perform a downsampling operation along the spatial dimensions (width, height), resulting in volume such as 
[16x16x12].

FC (i.e. fully-connected) layer will compute the class scores, resulting in volume of size [1x1x10], where each of the 
10 numbers correspond to a class score, such as among the 10 categories of CIFAR-10. As with ordinary Neural Networks and 
as the name implies, each neuron in this layer will be connected to all the numbers in the previous volume.
