# AnomalyDetectionProject
Deep Learning Application for Anomaly Detection in Railways

## Introduction
This main objective of this project is the development of fault detection schemesthat can accurately estimate possible abnormal operational patterns in railway systems leading to a reduction in LCC. Two achieve this, a set of anomaly detection schemes have been developed able to identify voltage variations, the fault location etc.

Anomaly detection refers to the process of finding unusual patterns that do not conform to expected
behavior. These unexpected behaviors are known as anomalies or outliers. There are three basic types of
anomalies, which are the point, the contextual and the collective anomalies. Specifically, if an individual
data instance is too far off from the rest of the dataset, then it is termed as point anomalous. Moreover, if
a data instance is anomalous in a specific context (usually in time series datasets), it is termed as
_contextual_ anomaly. Finally, if a set of related data is anomalous with respect to the whole dataset, then it
is known as _collective_ anomaly. 

We study the use of deep neural network based autoencoders, to identify anomalies in time series dataset. An __autoencoder__ is an unsupervised learning method that fits well with the purpose of identifying anomalies.

In particular, an autoencoder learns a representation of the input data in a large feature space, and
then performs dimensionality reduction, capturing the most representanive features, and then reconstruct the input data based on the features from the reduced feature space. Since anomalies
often correspond to non-representative features, an autoencoder trying to reconstruct these anomalies results in a large __reconstruction error__. Therefore data points with large reconstruction error
are considered anomalies.

## Implementation

We implemented 4 different deep autoencoders using __tensorflow__:
  *  Dense AutoEncoder
  *  Recurrent AutoEncoder(Seq to Seq)
  *  Convolutional AutoEncoder
  *  Denoising Convolutional AutoEncoder
