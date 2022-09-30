# Data-Mining-Algorithms-Applying
In this repository I added some of my projects in which I applied data mining algorithms on some open source databases. The algorithms are listed below.

* [Iris Dimentionality Reduction](https://github.com/kian79/Data-Mining-Algorithms-Applying/blob/main/README.md#iris-dimentionality-reduction)
* [Classification with Neural Network](https://github.com/kian79/Data-Mining-Algorithms-Applying/blob/main/README.md#classification-using-neural-network)
* [Clustering Algorithms](https://github.com/kian79/Data-Mining-Algorithms-Applying/blob/main/README.md#clustering-algorithms)
* [Association Rules](https://github.com/kian79/Data-Mining-Algorithms-Applying/blob/main/README.md#association-rules)

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

## Clustering Algorithms
THe goal of this project was to cluster the [make blobs dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_blobs.html). I used the following algorithms for clustering this dataset.
* K-means: To find the best K I used elbow technique and then clustered the dataset using the algorithm.
* DBSCAN: For some more complex data it was impossible to cluster using the k-means algorithm, so I used DBSCAN for this kind of data. To do so, I went through the following steps.
  * Determining the value of the epsilon
  * Determining the value of the MinPts

After clustering the data using both these algorithms, I compared the results and came to the conclusion that the second algorithm (DBSCAN) is better for data that can't be divided using lines. It is good for situations in which we want to divide the data based on density.

## Association Rules
In this project, I implemented association rules exraction. The parameters of this project are explained below.
* Support: Popularity of an item based on its frequency in the transactions.
* Confidence: The confidence(A->B) is the likeliness of of occurence B when A already happened. 
* Lift: Lift(A->B) controls for the support (frequency) of consequent while calculating the conditional probability of occurrence of {Y} given {X}.

Using the [mlxtend library](https://github.com/rasbt/mlxtend) I employed the apriori algorithm for implementing association rules.
