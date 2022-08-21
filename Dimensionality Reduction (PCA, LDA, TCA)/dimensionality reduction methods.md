 # Dimensionality reduction methods
 ## PCA-
 * Principal Component Analysis or PCA for short is a commonly used unsupervised linear transformation technique. 
 * PCA reduces the number of dimensions by finding the maximum variance in high dimensional data.
 * PCA reduces dimensions by looking at the correlation between different features. This is done by creating orthogonal axes – or principal components – with the direction of maximum variance as a new subspace.
 ### PCA steps-
 * Construct the covariance matrix by taking the joint covariance – or correlation in some cases – between each pair in the given vector.
 * Compute eigenvectors and eigenvalues of the matrix.
 * Sort the eigenvalues by decreasing order to rank the eigenvectors.
 * Get the k eigenvectors which corresponds to the k largest eigenvalues.
 * Construct a projection Matrix from the top k eigenvectors.
 * Transform the original input dataset with the newly created projection.
 ## LDA-
 * Linear Discriminant Analysis or LDA for short is a supervised method that takes class labels into account when reducing the number of dimensions. 
 * The goal of LDA is to find a feature subspace that best optimizes class separability.
 * It contains a “pre-processing” step calculating mean vectors from the class labels before extracting the eigenvalues.
 ### LDA steps-
 * For each class label: compute the d-dimensional mean vector
 * Construct a scatter matrix within each class, and between each class.
 * sum up the three individual scatter matrices into one final matrix.
 ## TCA-
 * This approach makes it possible to apply clustering algorithms to find decompositions of transformation programs at the method level.
