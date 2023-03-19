# Handwritten_Kmeans
Kmeans is an unsupervised algorithm, used for clustering data. This algorithm classifies data based on the average distance in a class.
Each cluster has a centroid and the algorithm update each centroid based on it's corrisponding callacified data's average coordinates. Until we don't see that much of a shift in the centroids' position the classification continues. <br/>
This project shows how Kmeans algorithm works. We used a dataset with 500 points and their Two-dimensional coordinates. In the diagram below you can see the destrebution:

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="">
 <img alt="Shows an light background in light color mode and a dark background in dark color mode." src="">
</picture> <br/>

## Table of contant
- [Centroid Functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#Centroid-Functions) <br/>
- [Main Functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#Main-Functions) <br/>
- [Hyperparameter Tuning (K)](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#set-hyperparameter) <br/>
- [Train & Evaluation](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#kmeans-execution) <br/>

## Centroid Functions
Centroids are imaginary points that indicate the classes. The first time we could choose where the centroids would be by default, or choose a data point randomly between the data we already have. The points assigned to the centroid would set how much the centroids will shift their position in the diagram and we classify the dataset baced on new centroids again. After some time and repitation, the shifts will be unnoticeable then we can say the centroids are set. <br/> 

- distance_calculator: we need a Euclidean distance function for classifing the dataset. <br/>
- centriods_changelog: saves the newly set centroids coordinates for the other functions to analyse. <br/>
- centriod_initialzation: initialize K number of random data point in our dataframe as centroids. <br/>
- assign_centriods: assign the nearest centroid to each data point baced on the least distance between the data and centroids. <br/>
- update_centroids: with the set points for each centroid, we can update the cordinates of where the centroid more likely to be. <br/>
- centroids_analysis: checks how much each centriod changed their position baced on the history. <br/>
- clusters_check: will edit the distance of each data and centroid and return average distance. <br/>

are the minor functions 
## Main functions
- plot function <br/>
This plotter shows the centroids and every cluster separate and with a different color. 
- Kmeans <br/>
This function is the main function. You can set K as the number of centroids, a centroid history and dataframe as input.


## Hyperparameter Tuning (K)
Kmeans loss is determined by how much distance there is. For tuning K as the number of centroids for a dataset, we can plot a 2D diagram of 3 to n centroids and check which one is more convenient for us. This dataframe is simple, so we only checked up to 10 centroids. The diagram showed 7 was a good choice.

## Train & Evaluation
The only thing left is executing the Kmeans function with seven centroids. 
