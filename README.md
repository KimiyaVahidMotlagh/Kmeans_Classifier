# Handwritten_Kmeans
Kmeans is an unsupervised algorithm, used for clustering data. This algorithm classifies data based on the average distance in a class.
Each cluster has a centroid and the algorithm update each centroid based on loss until we don't see that much of a shift in the centroids' position.
This project shows how Kmeans algorithm works. We used a dataset with 500 points 


## Table of contant
- [Main Functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#Main-Functions) <br/>
- [Kmeans functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#kmeans-function) <br/>
- [Hyperparameter Tuning (K)](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#set-hyperparameter) <br/>
- [Train and Evaluation](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#kmeans-execution) <br/>

## Main Functions
Centroids are imaginary points that indicate the classes. The first time we could choose where the centroids would be by default, or choose a data point randomly between the data we already have. The points assigned to the centroid would set how much the centroids will shift their position in the diagram. After some changes, the shifts will be unnoticeable then we can say those centroids set. <br/> <br/>

- centriods_changelog: resets the previosly saved centroids. <br/>
- centriod_init: initialize a random data point in our dataframe as centroids. <br/>
- assign_centriods: assign the nearest centroid to each data point. <br/>
- update_centroids: with the set points for each centroid, we can update the cordinates of where the centroid more likely to be. <br/>
- centroids_analysis: checks how much each centriod changed their position. <br/>
- clusters_check: will edit the distance of each data and centroid and return average distance. <br/>

are the minor functions 
## Kmeans functions
- plot function <br/>
This plotter shows the centroids and every cluster separate and with a different color. 
- Kmeans <br/>
This function is the main function. You can set K as the number of centroids, a centroid history and dataframe as input.


## Hyperparameter tuning
Kmeans loss is determined by how much distance there is. For tuning K as the number of centroids for a dataset, we can plot a 2D diagram of 3 to n centroids and check which one is more convenient for us. This dataframe is simple, so we only checked up to 10 centroids. The diagram showed 7 was a good choice.

## Kmeans execution
The only thing left is executing the Kmeans function with seven centroids. A job all done :)
