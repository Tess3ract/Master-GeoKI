# Master-GeoKI


## Related Master Thesis

This repository shows the results of the master thesis Classification of
Roof Materials from Aerial Images Using Machine Learning Methods by Moritz Niederer. The master thesis was obtained at the Saarland University of Applied Sciences (htw saar) in the course of studies Practical Computer Science of the Faculty of Engineering. It was supervised and reviewed by Prof. Dr.-Ing. Klaus Berberich and Prof. Dr.-Ing. Peter Birkner.



## Description
Roof material classification is the task of identifying the type of material used to cover the
roof of a building, such as asphalt, metal or tile . Roof material classification has various
applications, such as disaster management, urban planning, insurance, and environmental
monitoring. For example, roof material information can help assess the vulnerability of
buildings to natural hazards, such as fire, wind, or hail. Roof material classification can
also provide insights urban planning, such as the waste water system of a city.
Traditionally, roof material classification is performed by manual inspection, which is
time-consuming, costly, and prone to errors. Alternatively, roof material classification can
be automated by using remote sensing data, such as aerial or satellite imagery. However,
roof material classification from remote sensing data poses several challenges, such as the
variability of roof shapes, sizes, colors, textures, and orientations, as well as the presence
of occlusions, shadows, and noise.
In this project, we propose a novel approach to roof material classification from remote
sensing data based on deep learning and gradient boosting. Deep learning is a branch
of machine learning that uses neural networks with multiple layers to learn complex
and hierarchical representations of data. Gradient boosting is a technique that combines
multiple weak learners, such as decision trees, to form a strong learner that can achieve
high accuracy and generalization.
Our approach consists of two main steps. First, we design and train three convolutional
neural networks (CNNs) to extract features from remote sensing images and predict the
roof material labels. CNNs are a type of neural network that can effectively capture the
spatial and spectral information of images by using convolutional filters and pooling
operations. We use different architectures, input resolutions, and loss functions for each
CNN to capture different aspects of the roof material classification problem. In a second
step, we combine the predictions of the three CNNs and use them with other features as
input for a gradient boosted decision tree (GBDT) model. A GBDT model is an ensemble
of decision trees that are trained by adding new decision trees iteratively. Each added
decision tree specialises on the current error of the GBDT to iteratively reduce the errors.
We use a GBDT model because it can learn complex and non-linear relationships between
the input features and enables us to combine the predictions of multiple CNNs with other
data.
We evaluate the performance of our approach with cross validation and an realistic use
case example.

## Content of the Repository
This repository contains four Jupyter Notebooks:

### Preprocessing_main_data.ipynb
This notebook shows the preprocessing process of the data. This involves sending requests to a WMS server to obtain the orthophotos and applying filtering and feature generation techniques and extracting the roof images from orthophotos.

###  CNN_From_Scratch.ipynb
This notebook shows the implementation and training process of the CNN trained from scratch.

###  CNN_Transfer_Learning.ipynb
This notebook shows the implementation and training process of the CNN with Transfer Learning.

### GBDT.ipynb
This notebook shows the implementation and training of the gradient-boosted decision tree model. Additionally, we evaluate and select features to achieve optimal results in our GBDT model.

