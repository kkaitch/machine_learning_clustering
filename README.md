## Project Goal
This project is to play with unsupervised machine learning, using k-menas clustering to explore the basics of a face recognition system.

## Introduction
This project has three parts:

* Part I: Data Preprocessing and Exploration
* Part II: k-Means Clustering
* Part III: PCA and Eigenfaces

## Dataset
1. Faces in the Wild data set (roughly 250MB)
2. My image

## Key Findings
* K-Means effectively grouped faces with similar features
The algorithm was able to cluster facial images into groups that shared visual patterns, showing that K-Means can detect meaningful structure in high-dimensional image data without supervision.

* Dimensionality reduction was crucial
Applying PCA (Principal Component Analysis) before clustering dramatically reduced computation time and improved cluster separability. This step was essential for handling the high dimensionality of image pixels.

* Optimal cluster number aligned with subject count
Choosing a number of clusters close to the actual number of individuals in the dataset produced the most interpretable results, supporting the use of elbow plots or silhouette scores for determining k.

* Clusters captured identity and expression patterns
Some clusters grouped faces by identity, while others reflected differences in facial expression or lighting. This highlights both the strength and limitation of unsupervised clustering—the model groups by visual similarity, not necessarily semantic identity.

* Limitations in accuracy for face recognition tasks
While clustering offered useful insights, it lacks precision for facial recognition compared to supervised methods. For applications requiring exact identity matching, models like CNNs would be better.

