# Handwritten_Kmeans
Simple Kmeans algorithm executed in Python :)
Kmeans is an unsupervised algorithm, used mostly for clustering. This algorithm classifies data points based on the average distance in a class.
Each cluster has a centroid and the algorithm update each centroid based on loss until we don't see that much of a shift in the centroids' position


## Table of contant
- [Centroid set](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#centroid-set) <br/>
- [Kmeans functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#kmeans-function) <br/>
- [Hyperparameter tuning (K)](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#set-hyperparameter) <br/>
- [Kmeans execution](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#kmeans-execution) <br/>

## Centroid set
Centroids are imaginary points that indicate the classes. The first time we could choose where the centroids would be by default, or choose a data point randomly between the data we already have. The points assigned to the centroid would set how much the centroids will shift their position in the diagram. After some changes, the shifts will be unnoticeable then we can say those centroids set. <br/> <br/>
- centriods_changelog: resets the previosly saved centroids. <br/>
- centriod_init: initialize a random data point in our dataframe. <br/>
- assign_centriods: assign the nearest centroid to each data point. <br/>
- update_centroids: with the set points for each centroid, we can update the cordinates of where the centroid more likely to be. <br/>
- centroids_analysis: checks how much each centriod changed their position. <br/>
- clusters_check: will edit the distance of each data and centroid and return average distance. <br/>

are the minor functions 
## Kmeans functions

## Hyperparameter tuning

## Kmeans execution
