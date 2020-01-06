# Understanding-K-NN

### 1. What is it?:

K Nearest Neighbour is a simple algorithm that stores all the available cases and classifies the new data or case based on a similarity measure. It is mostly used to classifies a data point based on how its neighbours are classified.

'k’ in KNN is a parameter that refers to the number of nearest neighbours to include in the majority of the voting process.

### 2. How it works?

For each data-point in training data we find its distance from the given query point and select the k data-points with least distance. From these k data-points we do a majority vote and based on that we identifie out target variable yq.

If its a regression problem then we find the nearest pairs of Xq and yq and get the mean or median of these yq.

For numerical variables we can use different distance measures such as euclidean, manhattan, minkowski and for categorical features we should be using hamming distance.

### 3. How to choose best K?

Through K-fold cross-validation, generally 10 fold.

### 4. Pros and cons:

Pros:
- Simple to implement
- Flexible to feature/distance choices
- Naturally handles multi-class cases

Cons:
- Time complexity: O(nd)
Computation cost is quite high because we need to compute the distance of each query instance to all training samples
- Space complexity: O(nd)
Storage of data

Reference: https://towardsdatascience.com/a-simple-introduction-to-k-nearest-neighbors-algorithm-b3519ed98e

