# Behavior-Aware Network Segmentation using IP Flows
A dataset and analyses for a paper Behavior-Aware Network Segmentation using IP Flows

## Abstract

Network segmentation is a powerful tool for network defense. In contemporary complex, dynamic, and multilayer networks, network segmentation suffers from lack of visibility into processes in the network which results in less strict segment definition and loosen network security. Moreover, the dynamics of the networks makes the manual identification of network segments nearly impossible. In this paper, we inspect the possibilities of the behavior-aware network segmentation using IP flows and machine learning approaches that would enable to identify segments automatically even in a complex network. We evaluate the suitability of clustering algorithms for identification of behavior-consistent segments in a network. We show that the clustering algorithms can identify relevant behavior-consistent clusters that overlap with those identified manually by experts. Apart from the segment identification, we investigate the other essential task of network segmentation process: assignment of an unknown host to an existing segment. We evaluate the performance of four different classification mechanisms on a real-world dataset. We show that it is possible to assign an unknown host to an appropriate network segment with up to 92\% precision. Moreover, we release the whole dataset and experiment steps available for public use.

## Prerequisities

* Jupyter notebook (http://jupyter.org/)
* Python 3 (https://www.python.org/)
* Numpy (http://www.numpy.org/)
* Pandas (https://pandas.pydata.org/)
* Matplotlib (https://matplotlib.org/)
* Seaborn (https://seaborn.pydata.org/)
* Scikit-learn (http://scikit-learn.org/)
* imbalanced-learn (https://pypi.org/project/imbalanced-learn/)
* Cython (http://docs.cython.org/en/latest/index.html)


## Setup

1) 1) Go to `dataset/` directory 
    ```
    $ cd dataset/
    ```

2) Download dataset from [Zenodo webpage](https://zenodo.org/record/2669079) to `datset/` folder
    ```
    $ wget https://zenodo.org/record/2669079/files/host-network-traffic-time-series-2019-01-annon.csv
     ```
 
3) Go to `analyses/` directory
   ```
    $ cd analyses/
   ```
4) Run Jupyter notebook
    ```
    $ jupyter notebook
    ```

5) Run `Dataset_preprocessing.ipynb` to preprocess dataset

6) Run `Balancing_dataset.ipynp` to prepare balanced dataset

7) Run any of the analyses present in folders. 


## Acknowledgement

This research was supported by the Technology Agency of the Czech Republic under No. TA04010062 "Research and Development of Advanced Analytics Tools for Security and Performance Analysis of Network Infrastructure, Applications and Services". 