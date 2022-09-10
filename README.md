# Data-Mining-Algorithms-Applying
In this repository I added some of my projects in which I applied data mining algorithms on some open source databases. The algorithms are listed below.

* Iris Dimentionality Reduction
* Classification with Neural Network
* Clustering Algorithms
* Association Rules

## Iris Dimentionality Reduction
The goal of this project was to apply some preprocessing tools on IRIS dataset and then reduce its dimention using PCA. 
In the pre-processing phase of this project I did the following actions:
* Dropped null rows.
* Used label encoder to convert categorical feature to numerical feature.
* Normalized data using standart scaler.
* Applied PCA to reduce the number of features to 2.
* Plot the output dataframe to see the changes.

## Classification using Neural Network
In this project I trained a neural network using Keras library. To emphadize the effect of different variables of the neural network, it was trained step by step. In the first steps I trained a neural network using no activation function and a linear activation function. The results are very bad as expected. After that trained the neural network with a relu activation function but with a bad learning rate. After finding the optimum learning rate I achieved a 97% accuracy on the fashion MNIST dataset.
