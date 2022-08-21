# KNN
* K-Nearest Neighbor (K-NN) is an instance-based (memory-based) algorithm.
* K-NN is based on the fact that the similar objects lie in the close proximity to each other in the feature space.
## KNN steps-
* K-Nearest Neighbor algorithm works in the following steps:
* Determine parameter K = number of nearest neighbors.
* Calculate the distance between the query-instance and all the training samples.
* Sort the distance and determine nearest neighbors based on the K-th minimum distance.
* Gather the category Y of the nearestneighbors.
* Use simple majority of the category of nearest neighbors as the label of the query instance in case of classification and average of the values of k nearest neighbors in case of regression.
## How to set value of K
* In KNN, finding the value of k is very crucial. A small value of k means that noise will have a higher influence on the result and a large value make it computationally expensive.
* If we choose our K = 1 , then our algorithm behaves as over fitting and it gives a non - smooth decision surface.
* As K increases, our decision surface gets smoother and, if we choose K as very large, then our algorithm behaves as underfitting and it gives a smooth decision surface and everything becomes one class which is the majority class in our dataset.
## Advantages of KNN-
### Prediction quality:
* A kNN classifier is able to recover unstructured partitions of the space, as opposed to, say, a linear classifier that requires a linear separation between the classes.
* It can also adapt to different densities in the space, making it more robust than methods such as support vector machine (SVM) classification with radial basis function (RBF) kernel.
### Short cycles:
* Another advantage of kNN is that there is little to no training involved.
* This means that iterating over different possible metrics / modifications of the input dataset is potentially faster when compared to a classifier that requires a heavy training procedure.
### Multi-Class Classification:
* kNN can seamlessly handle a very large number of classes.
* For comparison, a linear model or a deep neural network with a cross-entropy loss must explicitly compute a score for each possible class, and choose the best one.
## Limitations of K-NN Algorithm
* Costly inference:
* The major disadvantage of kNN is its costly inference.
* To infer the label of an input query, we must find the data points closest to it.
* A naive solution would keep all data points in memory, and, given a query, compute the distance between it and all data points.
* For concrete quantities, if the training set contained n data points of d dimensions, this process requires O(nd) arithmetic operations per query and O(nd) memory.
