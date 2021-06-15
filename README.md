# Cifar10_AutoEncoder
An autoencoder based on a deep CNN architecture is trained on the cifar10 dataset to reproduce the images.

# How To Use This Repository:
Simply open the .ipynb file in either Jupyter notebooks or colab or any other place you like and follow along.

## Here's a summary of the architecture used :

    _________________________________________________________________
    Layer (type)                 Output Shape              Param #   
    =================================================================
    input_2 (InputLayer)         [(None, 32, 32, 3)]       0         
    _________________________________________________________________
    conv2d_7 (Conv2D)            (None, 32, 32, 64)        1792      
    _________________________________________________________________
    max_pooling2d_2 (MaxPooling2 (None, 16, 16, 64)        0         
    _________________________________________________________________
    conv2d_8 (Conv2D)            (None, 16, 16, 128)       73856     
    _________________________________________________________________
    max_pooling2d_3 (MaxPooling2 (None, 8, 8, 128)         0         
    _________________________________________________________________
    conv2d_9 (Conv2D)            (None, 8, 8, 256)         295168    
    _________________________________________________________________
    conv2d_11 (Conv2D)           (None, 8, 8, 128)         295040    
    _________________________________________________________________
    up_sampling2d_2 (UpSampling2 (None, 16, 16, 128)       0         
    _________________________________________________________________
    conv2d_12 (Conv2D)           (None, 16, 16, 64)        73792     
    _________________________________________________________________
    up_sampling2d_3 (UpSampling2 (None, 32, 32, 64)        0         
    _________________________________________________________________
    conv2d_13 (Conv2D)           (None, 32, 32, 3)         1731      
    =================================================================
    Total params: 741,379
    Trainable params: 741,379
    Non-trainable params: 0
