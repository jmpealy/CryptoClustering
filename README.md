# Clustering cryptocurrencies with Machine Learning (*Challenge 19*)

This repository contains a mini-project in which a K-means model was used to cluster different cryptocurrencies.

## Author

Jason Pealy: [https://github.com/jmpealy]

## Overview of the Analysis

In this project, an unsupervised Machine Learning model was applied to cluster returns (%) for various cryptocurrencies. The purpose of the analysis was to find the best way to cluster such currencies and to evaluate how inertia and the number of features (components) affect the analysis.

The data were prepared for the analysis, and the following method was run twice:
- Creating a ```Pandas``` DataFrame with the data to be analysed, finding the best value for 'k', clustering the cryptocurrencies with the K-means component of ```Sci-kit Learn```, and plotting the results with ```hvPlot```.

It was run twice because two different datasets were used: first, the original dataset, and second, the same dataset, but optimised with a principal compenent analysis (PCA).

## Questions answered

As you will see in the Crypto_Clustering jupyter notebook file in the repository, the following 5 questions were answered as the analysis was conducted:

1. Question: What is the optimal value for k? Answer: It appears to be 4. (original dataset)

2. Question: What is the total explained variance of the three principal components? Answer: Roughly 89.5%. (dataset after applying PCA)

3. Question: What is the optimal value for k when using the PCA data? Answer: It still looks to be 4. (dataset after applying PCA)

4. Question: Does it differ from the optimal k value found using the original data? Answer: No, it doesn't. (dataset after applying PCA)

5. Question: After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means? Answer: The inertia decreased and the data points seem to be less dispersed. Reducing the number of features to cluster the data does decrease the inertia (slightly) and seems to cause a bit less dispersion among the data points.  Having fewer features to cluster the data seems like it reduces ambiguity around the data which should lead to a better interpretation of the results (original dataset vs the same dataset after PCA applied).

## Contents of the repository

### The *Resources* folder:

Contains the CSV file with the crypto return data used in the analysis

### The *Images* folder:

Contains png image files of the various plots created within the jupyter notebook file using hvplot

### The *Crypto_Clustering.ipynb* Jupyter Notebook:

It contains the ```Python``` code used for the analysis. All the code has been commented, so it's easier to understand.

### A text file with a couple of web links to references I used for help in writing my code.

## Data Reference

The dataset was generated by [edX Boot Camps LLC](https://www.edx.org/boot-camps).

```#Thank you for reading me!```
