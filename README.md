# ResNet for CIFAR-10 Classification  
This repository contains a Residual Neural Network (ResNet) implemented in PyTorch for the task of classifying images from the CIFAR-10 dataset.  

## Data  
The CIFAR-10 dataset consists of 32x32 pixel color images in 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck).  

## Model Architecture  
The ResNet architecture consists of multiple residual blocks, each containing two convolutional layers with batch normalization and ReLU activation. The network utilizes skip connections to overcome the vanishing gradient problem, allowing for more straightforward training of deep networks.  

## Initialization  
Weights in the convolutional layers are initialized using the standard method, and the learning rate is decayed every 20 epochs.  

## Training  
The model is trained for 25 epochs with a batch size of 100. The Adam optimizer is used with a learning rate of 0.001, and Cross Entropy Loss is employed as the loss function.  

## GPU Support  
The code checks for the availability of a CUDA-compatible GPU and moves the model to the GPU if present.  

## Evaluation  
After training, the model is evaluated on the test set. The accuracy of the model on the test set is calculated, providing a performance metric for the trained ResNet.  

## Results  
The script prints the training loss at regular intervals and decays the learning rate every 20 epochs. After training, it evaluates the accuracy of the model on the test set.  

