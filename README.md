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

1) Go to `dataset/` directory 
    ```
    $ cd dataset/
    ```

2) Download dataset from [Zenodo webpage](https://zenodo.org/record/2669079) to `dataset/` folder
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

7) Go to `DTW_LB_Keogh/` directory
   ```
    $ cd DTW_LB_Keogh/
   ```

8) Run `DTW_module.ipynb`. Rename generated **.so** file to **DTW.so** and copy this file into `analyses/KNN_LB_Keogh/` and `analyses/K-Means/` directories

9) Run any of the analysis present in folders. 

## How to cite

Juraj Smeriga and Tomas Jirsik. 2019. Behavior-Aware Network Segmentation using IP Flows. In Proceedings of the 14th International Conference on Availability, Reliability and Security (ARES '19). ACM, New York, NY, USA, Article 5, 9 pages. DOI: https://doi.org/10.1145/3339252.3339265 

**Bibtex**

```
@inproceedings{Smeriga:2019:BNS:3339252.3339265,
 author = {Smeriga, Juraj and Jirsik, Tomas},
 title = {Behavior-Aware Network Segmentation Using IP Flows},
 booktitle = {Proceedings of the 14th International Conference on Availability, Reliability and Security},
 series = {ARES '19},
 year = {2019},
 isbn = {978-1-4503-7164-3},
 location = {Canterbury, CA, United Kingdom},
 pages = {5:1--5:9},
 articleno = {5},
 numpages = {9},
 url = {http://doi.acm.org/10.1145/3339252.3339265},
 doi = {10.1145/3339252.3339265},
 acmid = {3339265},
 publisher = {ACM},
 address = {New York, NY, USA},
} 
```

## Acknowledgement

This research was supported by ERDF "[CyberSecurity, CyberCrime and Critical Information Infrastructures Center of Excellence](https://www.muni.cz/en/research/projects/41145)" (No. CZ.02.1.01/0.0/0.0/16\_019/0000822).  
