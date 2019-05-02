# Analyses 

This folder contains subfolders with following analyses:

## Dataset preprocessing

These notebooks include required dataset preprocessing needed to be done before analyses are executed.

* `Dataset_preprocessing.ipynb` - includes steps for dataset preprocessing such as missing value handling, outlier removal, etc.
* `Balancing_dataset.ipynb` - includes steps for dataset balancing - undersampling of the majority class.

## Network Segment Discovery

* **K-means** - includes K-means clustering notebooks on all subnets, selected subents, and binary clustering.  
* **K-means_LB_Keogh** - includes K-means clustering with LB-Keogh measure as distance metrics. Notebooks include clustering on all subnets, selected subents, and binary clustering
* **DBSCAN** - includes density-based spatial clustering of applications with noise on all subnets, selected subents, and binary clustering.

## Network Segment Assignment

* **KNN** - includes K-nearest neighbour classification notebook. The classification is executed on all subnets, selected subents, and two subnets.
* **KNN_LB_Keogh** - includes K-nearest neighbour classification using  LB-Keogh measure as distance metrics notebook. The classification is executed on all subnets, selected subents, and two subnets.
* **SVM** -  includes support vector classification using  LB-Keogh measure as distance metrics notebook. The classification is executed on all subnets, selected subents, and two subnets.
* **DTs** - includes decision tree classification notebook. The notebook contains classification on all subnets, selected subents, and two subnets.
