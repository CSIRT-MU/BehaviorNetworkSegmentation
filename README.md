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

## Analyses

Analyses are present in __analyses__ directory. To run an analysis yourself, you need to start your own Jupyter notebook session and load selected analysis.

## Acknowledgement

