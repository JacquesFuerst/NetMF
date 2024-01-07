# NetMF

In this repository, the aim was to reproduce the results of the study 'A Comparative Study for Unsupervised Network
Representation Learning' [1]. The focus lies specifically on the NetMF method, as first introduced in 'Network Embedding as Matrix Factorization: Unifying DeepWalk, LINE, PTE, and node2vec'[2]. The two tasks that the the method is evaluated on are node classifcation and link prediction.

## Files-overview

### NetMF_implementation-final.ipynb

This notebook file contains code to create a NetMF embedding in form of a .npy file, when used in google Colab, mounting a Google Drive repository. The parameters were set as in the original study [1]. The embedding can be created for any dataset from the pytorch_geometric library or .csv files as can be found on the datasets provided by the Arizona state university [3].

### Link_prediction-final.ipynb

Link prediction implementation for experiments on the NetMF embeddings. Works based on the embeddings in form of .npy files.

### Node_classifcation-final.ipynb

Node classification implementation based on the code provided by the authors of [2]. Works based on the embeddings in form of .npy files.

### .npy files

These represent the NetMF embeddings created through running NetMF_implementation-final.ipynb for the respective datasets.

## Omitted datasets

The Youtube, BlogCatalog and Flickr datasets could not be uploaded due to the .csv files being larger than 25GB. They can be found under the following links:

Youtube: http://datasets.syr.edu/datasets/YouTube2.html

Flickr: http://datasets.syr.edu/datasets/Flickr.html

BlogCatalog: http://datasets.syr.edu/datasets/BlogCatalog3.html

# References
[1] M. Khosla, V. Setty, and A. Anand, “A comparative study for unsupervised network representation learning,” IEEE Transactions on Knowledge and Data Engineering, vol. 33, no. 5, pp. 1807–1818, 2019.

[2]  J. Qiu, Y. Dong, H. Ma, J. Li, K. Wang, and J. Tang, “Network embedding as matrix factorization: Unifying deepwalk, line, pte, and node2vec,” in Proceedings of the eleventh ACM international conference on web search and data mining, 2018, pp. 459–467.

[3] A. S. University, “Datasets,” http://datasets.syr.edu/pages/datasets.html.
