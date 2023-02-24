# customer-clusterization

<div align="center">
  
![customer-segmentation](img/customer-segmentation.jpg)
  
</div>

## Introduction 

The objective of this project to **segment customers** from a automobile clients database. Since we don't have labels for our instances, it is an **unsupervised** problem, and more specifically, a **clusterization**.

## Context and business

Segmenting clusters can aid businesses by helping to create strategies to a specific group of clients. Those can be used to identify valuable customers, target campaings, etc.

## Model

I've employed the `K-Prototypes` as the clusterization algorithm since our data is mixed between numerical and categorical features. Unfortunately this limit us when chosing techniques to find the best number of clusters. Despite this, the **elbow method** was succefully used to get the ideal number of clusters $k = 4$.

## Results

We segmented our client database in four clusters which are summarized as:

> **Cluster 0**: Low spending, never married, not graduated, healthcare workers, younger;

> **Cluster 1**: Low/Average spending, mostly females, highest work experience;

> **Cluster 2**: Artists/Entertainers, married, graduated;

> **Cluster 3**: High spending, married, lawyers, older;


Some potential strategies that can be suggested based on this segmentation are

* There is potential to create strategies to expand spending in Cluster 0. The cluster is particularly well described and plans to target those clients can be very precise. In contrast, Cluster 3 contains clients that already have high spending;

* Specific campaigns to women can be created to clients in Cluster 1;
