# Clustering

## Background Introduction
- Definition of clustering
- Some examples and cases of clusternig in the real life
- Difference between classification and clustering

## Unsupervised Learning
- Definition of unsupervised learning
- Pros and cons compared with supervised learning in general
- Lead to K-Means Algorithm

## K-Means Algorithm from Scratch
- Dataset

    1. Self-generated Data: relatively easy, could generate simple plot during each iteration and could be understood more easily (Personally prefer this)
    2. MNIST: more difficult, might need GPU

- Simple introduction of K-Means Algorithm

    1. Randomly choose clusters at first
    2. Assign every point to the closest cluster (minimum loss)
    3. Within each cluster, find the best representative point
    4. Iterate Step 2, 3 until certain condition is met
- How to choose the number of cluster

    1. Plot the dataset and check with eyes
    2. "Elbow" method (mentioned later)
- Loss function

    1. Definition
    2. Rule: non-negative, symmetric, triangle inequality
    3. Common used: Euclidean, Manhattan...
    4. Write Euclidean distance as a function
    5. When using Euclidean, talk about the gradient + gradient descent
- Plot

    1. The representative point of each cluster is marked by "x"
    2. Each cluster has its own colour

- Implement the whole algorithm step by step

## K-Means Algorithm using Sklearn
- Implement the algorithm using Sklearn and compare with the hand-written one

## Get Better Result
- "Elbow" method: plot the loss and find the "elbow" of the line
- Silhouette Score

    1. Definition
    2. Implementation using sklearn
- The limitation of the K-Means: strongly affected by the outlier
- Alternatives: K-Means++, K-Medoids (PAM)

## Summary
- Definition of clustering and unsupervised learning
- Famous algorithm: K-Means
- General Pipeline of ML: find data, train, optmize loss function, repeat until certain condition is met
- How to get better result: check the loss function, evaluate certain metrics, change the method...