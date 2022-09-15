#Technical Report

DataSet:

The dataset here is MNIST.The MNIST dataset is a large dataset of handwritten digits that is commonly used for training various image processing systems.the data set was imported from keras.

Initialization of weights:

Weights and bias are initialized by randomly by using numpy.  Functions for forward propogation and for  backword propogations are defined

Forward and backward propagation is very important to learn machine learning.In general, feedforward means moving forward with provided input and weights till the output.And, backward propagation is moving from ouput to input.

Activation Function:
 I will try to compare and analysis Sigmoid( logistic) activation function with others like Tanh, ReLU, Leaky ReLU, Softmax activation function. These all are activation function used generally in Neural Network algorithm and deep learning

The information moves from the input layer to the hidden layers. In a simple case of each layer, we just multiply the inputs by the weights, add a bias and apply an activation function to the result and pass the output to the next layer. We keep repeating this process until we reach the last layer.

1.Sigmoid Activation Function:
Sigmoid Activation function is very simple which takes a real value as input and gives probability that ‘s always between 0 or 1. It looks like ‘S’ shape.

2. Tanh or Hyperbolic tangent:Tanh help to solve non zero centered problem of sigmoid function. Tanh squashes a real-valued number to the range [-1, 1]. Here I defined tanh function
3. ReLU (Rectified Linear Unit):
This is most popular activation function which is used in hidden layer of NN. It provides the same benefits as Sigmoid but with better performance.
4. Leaky ReLU
It prevents dying ReLU problem.T his variation of ReLU has a small positive slope in the negative area, so it does enable back-propagation, even for negative input values
Network class is defined by creating add ,loss,predict and fit functions
DataPreprocessing:
For image preprocesing, reshaped the image and divided it with 225 to get normalized images
Network:
For building of networks,three fully connected hidden layers with activation function as tanh as taken.Here 10 epochs are taken which gave error of 0.0079
F1score: F1 score for training data is 0.97 and F1 score for test data is 0.96
