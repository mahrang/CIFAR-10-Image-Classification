# CIFAR-10 Image Classification

The CIFAR-10 dataset contains 60,000 32x32 color images of 10 different classes, with 6,000 images of each class.  
The classes are:  airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck.  The classes are mutually exclusive.  
There is no overlap between automobiles and trucks.  Neither class includes pickup trucks.  
The dataset is divided into 2:  one training dataset containing 50,000 images and one test dataset containing 10,000 images.  
The training dataset contains 5,000 images of each class and the test dataset contains 1,000 images of each class.  
The CIFAR-10 dataset is available at http://www.cs.toronto.edu/~kriz/cifar.html

It can also be imported using the Keras library, as is done in the code.

Here are images from each class in the dataset:

![Image of Each Class](https://github.com/user-attachments/assets/556abb86-2a29-415b-beab-2879f56b99c5)

I classified the images in the CIFAR-10 dataset by building a multilayer perceptron (MLP) using TensorFlow, Scikit-Learn, and Matplotlib.
The MLP I built has 1 hidden layer containing 175 neurons and a ReLU activation function.  This MLP has a test accuracy of 52.42%.
To find the optimal number of neurons, I swept the number of neurons in the hidden layer from 100 to 800 in increments of 25 and plotted their training 
and validation errors.
175 neurons gave the lowest validation error, as shown by the plot below.

![Unknown](https://github.com/user-attachments/assets/6b0563f9-37ac-4317-bdda-7fad751e0756)

Relevant Paper:
Alex Krizhevsky, Learning Multiple Layers of Features From Tiny Images, April 2009. 
http://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf
