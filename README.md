# project-ML
Given an image, can we predict the correct class of this image? The images are very small (32x32) and by visualizing them you will notice how difficult it is to distinguish them even for a human. In this notebook we are going to build a CNN model that can classify images of various objects.



Dataset:-

The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.

1-

2- We have 10 classes of images (not from same type):

Label names --> Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck (but not pickup truck) 3- Different label not from same type. and optimizer "adam".



Result:-





Train Result :

 loss: 0.3286  accuracy: 0.8852  precision: 0.9130  recall: 0.8612

Validation Result :

 val_loss: 0.5349  val_accuracy: 0.8378  val_precision: 0.8674  val_recall: 0.8176 ‏"

Model:-

1-

We create CNN layers with filter 3*3 and we make use of maxpool function to take useful features from image.

2- Each CNN layer use activation function "relu".

3- After CNN layers we use flatten layer to convert output of CNN layer (2d) to vector.

4- We create neural network layer with 128 neurons.

5- Last layer is the output layer with 10 neurons with activation function "softmax".

6- We used loss function "categorical_crossentropy
