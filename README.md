# Handwritten_Kmeans
Kmeans is an unsupervised algorithm used for clustering data. This algorithm classifies data based on the average distance in a class.
Each cluster has a centroid. The algorithm updates each centroid based on its corresponding classified data's average coordinates. The loop continues until we don't see that much of a shift in the centroids' position. <br/>
This project shows how the Kmeans algorithm works. We used a dataset with 500 points and their Two-dimensional coordinates. In the diagram below you can see the distribution:

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="">
 <img alt="Shows a light background in light color mode and dark background in dark color mode." src="https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/Pictures/Data.jpg">
</picture> <br/>

## Table of content
- [Centroid Functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#Centroid-Functions) <br/>
- [Main Functions](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#Main-Functions) <br/>
- [Hyperparameter Tuning (K)](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#set-hyperparameter) <br/>
- [Train & Evaluation](https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/README.md#kmeans-execution) <br/>

## Centroid Functions
Centroids are imaginary points that indicate the classes. The first time we could choose where the centroids would be by default, or choose a data point randomly between the data we already have. The points assigned to the centroid would set how much the centroids will shift their position in the diagram and we classify the dataset based on new centroids again. After some time and reputation, the shifts will be unnoticeable then we can say the centroids are set. <br/> 

- distance_calculator: we need a Euclidean distance function for classifying the dataset. <br/>
- centriods_changelog: saves the newly set centroids coordinates for the other functions to analyze. <br/>
- centriod_initialzation: initialize K number of random data points in our dataframe as centroids. <br/>
- assign_centriods: assign the nearest centroid to each data point based on the least distance between the data and centroids. <br/>
- update_centroids: with the set points for each centroid, we can update the coordinates of where the centroid is more likely to be. <br/>
- centroids_analysis: checks how much each centroid changed its position based on history. <br/>
- clusters_check: will edit the distance of each data and centroid and return the average distance. <br/>

are the minor functions 
## Main functions
- plot_cluster<br/>
This plotter function shows the centroids and their cluster. Centroids are red and the classes are in different colors.
- k_means_clustering<br/>
This function uses the previously mentioned functions and is the main function. You can set K as the number of centroids. you need a centroid history and the dataframe as input. After the clustering is done, the function will output the centroids coordinates and the classified dataframe.


## Hyperparameter Tuning (K)
Kmeans loss is determined by how much distance there is. For tuning K as the number of centroids for a dataset, we can plot a 2D diagram of 3 to n centroids and check which one is more convenient for us. O8
ur dataframe is simple, so we only checked up to 10 centroids.

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="">
 <img alt="Shows a light background in light color mode and dark background in dark color mode." src="https://github.com/KimiyaVahidMotlagh/Handwritten_Kmeans/blob/main/Pictures/Elbow.jpg">
</picture> <br/>

The diagram shows that 7 was a good choice.

## Train & Evaluation
The only thing left is executing the Kmeans function with seven centroids. We don't have a way to evaluate our code with accuracy however we can evaluate the classification with our sight. Due to the randomized centroid initialization, you can re-run the code until you are satisfied with the clustering. 
