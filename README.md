# DenoisingAutouencoder_MNIST

## Requirements

## Import dataset
In this section we import the MNIST dataset from the keras library.

## Adding noise
As we want the network to be able to denoise images, we have to train it in noisy images. So we 
add a random normal noise to each image in the training set and we normalize the them.

## Defining the model
Here i define the architecture of the autoencoder. I use two convolutional layers each one followed by two max_pooling layers after that the data is encoded. So i added two upsampling layers followed by transpose convolutions. I used Adam optimizer and binary cross entropy as the loss function.

## Training the model
In this part i trained the model for 5 epochs with the noisy images as input and the normal images as output.

#Viewing the results
Here i load the best model saved while training and use it to denoise 3 random images in the test set. 



