# Ear-Recognition

#### -> The entire report (including results and a more detailed task description) is in provided pdf.<-

#### -> Data is in the awe folder <-

Implementation and evaluation of a popular old-school algorithm Local Binary Patterns (LBP) for the recognition task based on scientific papers. 
In order to see that implementation works we compared this to a plain pixel-wise comparison of images and also to the OpenCV’s implementation.

Things that were meant to do:

• A loop to read all the images in grayscale and in a fixed image size (e.g. 128×128) and then call feature extractor for each one.

• Plain pixel-by-pixel feature extractor (just transform twodimensional image into one-dimensional vector) to have some baseline.

• LBP feature extractor with multiple stages of implementation and add-ons, e.g.: with or without histograms, different radius levels.

• Compare all the computed feature vectors between themselves (you get a triangular matrix of distances) separately for each type of feature extractor (pixel-by-pixel, LBP) and compute rank-1 recognition rate. You do that by getting the closest vector to the currently observed
one and check whether it corresponds to the same class (correct) or not (incorrect). When you go through all the vectors and sum up predictions you get the percentage of
rank-1 recognition rate.


The goal was to answer following questions:

• Report rank-1 classification accuracy when using pixel-wise image comparison.

• Report rank-1 classification accuracy with your own basic version of LBP.

• Report on improvement/deterioration for each LBP improvement, such as:

– using histograms or not,

– using different radii,

– using different input image sizes,

– etc.

• Report on improvement/deterioration when using different distance measures for feature vector comparison(e.g. euclidean vs cosine distance).

• Compare rank-1 of your implementation with the one from OpenCV (Scikit).
