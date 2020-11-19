# Keras-examples

This is a collection of the examples I tried while learning to implement Neural Networks using Keras. The examples come from the book Deep Learning with Python.

###IMDB
Classifying movie reviews as positive or negative. Sentiment analysis. The model achieved 88% accuracy.
The network used 2 layers with relu activation and 1 with sigmoid, and a loss function binary_crossentropy.
This was the recommended model. I also experimented with removing a layer, adding a layer, making the layers bigger, changing the loss function, and changing the activation function. They all resulted in lower performance.

###news
Classifying new articles into their categories. a multi class classification problem. Achieved 78.5% accuracy.
The network used 2 layers with relu activation and 1 with softmax, and a loss function categorical_crossentropy.

###house prices
predicting house prices based on multiple factors in Boston in the 1970s. a regression problem.
The network used 2 layers with relu activation and 1 without, and a loss function MSE. Also used cross validation with 4 folds because the dataset is small.

###MNIST convent
classifying handwritten digits. an image processing multi class classification problem. Achieved 99% accuracy.
The network used 3 convolutional layers with relu activation, 2 maxpooling layers, a flatten layer, a dense layer with relu activation, and a dense layer with softmax activation, with a loss function categorical_crossentropy. Also used datagens to input the imgaes to the network.

###dogs vs cats
classifying images of cats and doggs. an image processing binary classification problem. Achieved 84% accuracy.
The network used 4 convolutional layers with relu activation, 3 maxpooling layers, a flatten layer, a dropout layer, a dense layer with relu activation, and a dense layer with sigmoid activation, with a loss function binary_crossentropy. Also used datagens to input the imgaes to the network.
To provide the model with more training data, I used image augmentaion.
