# SV-Learn: Learning Matrix Singular Values with Neural Networks

## About
This repo is a composite of the main scripts used to create models for the paper [Sv-Learn](https://ieeexplore.ieee.org/document/10031050).
Scripts for creating the data, training neural networks, and some data analysis is included. Though, this repository does not include code that was used 
for data-analysis in the paper, but has the essential models that were used experimentally to predict the singular-value-decomposition. 

``cifar-10.ipynb`` - Creates grayscale datasets based on CIFAR-10 images and trains a model using its corresponding SVD\
``uci-training.ipynb`` - Does the same except with UCI's Spambase dataset\
``poormans-svd.ipynb`` and ``poormans-svd-cifar.ipynb`` - Compares different methods in extrapolating the SVD in which our models were tested against\


## Abstract
>The singular value decomposition (SVD) factors a
matrix into three separate matrices: two (semi-)unitary matrices
whose columns are left/right singular vectors and one diagonal
matrix whose diagonal entries are singular values. Typically,
performing SVD on big matrices is taxing due to its compu-
tational complexity in the cubic order of its dimensions. With
the advances and rapid growth of deep learning techniques
in a broad spectrum of applications, a fundamental question
arises: can deep neural networks learn the singular values of a
matrix? To answer this question, we propose a novel algorithm,
namely SV-learn, to predict the singular values of a given input
matrix by leveraging the advances of neural networks. Numerical
results demonstrate that our proposed method outperforms the
competing alternatives in terms of achieving lower normalized
mean square error on singular value prediction when using real-
world datasets. Further, the predicted singular values combined
with singular vectors of an input data allow us to reconstruct
the input matrices with promising performance.

## Notes
If you plan on running this set yourself, please take into account the following:
- You must install the required libraries (included in *requirements.txt*)
- **Scripts will download and create up to 1GB of data** (in total, not individually)
- By default, the actual training is skipped over as ``/models`` already includes trained models
