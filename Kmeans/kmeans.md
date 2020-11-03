# K-means Clustering

## Unsupervised Clustering Algorithm
##### Stephen Kirby - October 20th, 2020

---
</br>

## Intuition

The K-means algorithm takes raw (unlabeled) data, partitions into a fixed set of groups (or **`clusters`**, **`k`**) based on the distance between samples in the **euclidean space**.

Clusters are defined by a central point called a **centroid**. Through iterative updating of these centroids and the respective sample points, the K-means algorithm will parse unlabeled data into significantly similar groups. 


## Process

Take an unlabeled set of data, like the sample space displayed below:




Each cluster represented by a **centroid**, which is selected randomly at first.

Cycle: 
1. K-means assigns each point to the centroid with the **closest mean**. 
2. Then, each centroid is updated by taking the mean of all points in it’s cluster. 

---
</br>

## Mathematics


---
</br>

## Application


