# Mini Project 3: Human Activity Recognition Using Smartphones
This project involves clustering human activities recognized through sensor data captured from smartphones. A group of 30 volunteers performed six activities, with their movements captured using the embedded accelerometer and gyroscope of a Samsung Galaxy S II. The aim is to categorize these activities into clusters to understand the patterns and characteristics of human movement.

## Dataset Description
The dataset, sourced from the UCI Machine Learning Repository, includes data from experiments carried out with volunteers aged between 19-48 years. The six activities performed are WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, and LAYING. Sensor signals were pre-processed and sampled in fixed-width sliding windows, with features extracted from both time and frequency domains

## Data Preprocessing
The preprocessing steps included standardizing the dataset to improve clustering algorithm performance. Despite the data being normalized, standardization was preferred as it is conducive to the algorithms' efficiency.

## Modeling

### Task 1: Clustering with K-Means and DBSCAN
- **K-Means**: The optimal number of clusters was determined using the elbow method, silhouette score, and Davies-Bouldin index, suggesting 2 as the optimal number.
- **DBSCAN**: Parameters such as epsilon and min_samples were optimized based on distance calculations and empirical processes.

### Task 2: Dimensionality Reduction
Three techniques were explored: PCA, t-SNE, and UMAP, to evaluate their impact on computational efficiency and clustering quality. These techniques significantly improved runtime performance and offered distinct visual separation of clusters.

### Task 3: Visualization of Clusters
The dimensionality reduction techniques facilitated the visualization of high-dimensional data in a two-dimensional space, revealing distinct clusters representing different human activities.

## Conclusion
The clustering revealed clear separation into two groups indicative of active (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS) and passive (SITTING, STANDING, LAYING) activities. This distinction aligns with the intrinsic differences in the nature of these activities. The project underscored the importance of dimensionality reduction and standardization in analyzing high-dimensional sensor data. Challenges such as choosing the appropriate dimensionality reduction technique and optimizing clustering parameters were overcome through methodical experimentation and analysis.

