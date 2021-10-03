Import two libraries first are TensorFlow library and the ImageDataGenerator class from Keras.Preprocessing.image module.


In the data preprocessing part we transform the the training and test images by using image augmentation method which is done by the the image data generator class.  This reduces overtraining that is overfitting of images while training.



while building the CNN model 

first we initialise the sequential class of models module

now we add the convolutional layer with the help of Conv2D class and apply ReLU activation function 

Next we use MaxPool2D class to add pooling layer to the neural network for getting better feature maps 

To enhance our feature maps we add second convolutional and pooing layers then we flatten it and then use a full connection layer by using Dense class of layers module and finally we add an output layer having an sigmoid activation function.



Before training the CNN model we will combine all the layers by using Adam optimizer and assign loss and metrics parameters as required

we train the CNN model by using the fit method and define the number of epochs. CNN model training is little bit different than other ML model's training.

To make a single prediction first we import the number library and then we import the image class from the the preprocessing soft module from the keras library reload the image  and assign it a target size which we use for input images by using load image method and assign it to test image 

by using image to  image to array method we convert the date image to matrix format

the matrix using 2D format but we have to

image to array, adding a fake dimension which corresponds to the batch size i.e.32 on which the model was trained done by using np.expand_dims

before deleting the test image matrix is divided by 255 as we applied teacher feature scaling to the training need assessment

training weight to stop class underscore in gives the interface of it class



