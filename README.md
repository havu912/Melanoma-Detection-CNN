
# Melanoma Skin Cancer Detection




## Problem Statement

Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Dataset

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


The data set contains the following diseases:

    1. Actinic keratosis
    2. Basal cell carcinoma
    3. Dermatofibroma
    4. Melanoma
    5. Nevus
    6. Pigmented benign keratosis
    7. Seborrheic keratosis
    8. Squamous cell carcinoma
    9. Vascular lesion
## Business Goals

Build a CNN based model which can accurately detect melanoma. The model being built is a multiclass classification model using a custom convolutional neural network in TensorFlow.
## Model Building
To detect melanoma, I build a multiclass classification model using a custom convolutional neural network in TensorFlow, following by:
1.  Importing Skin Cancer Data: loading images from drive
2.  Create a dataset: define some parameters for the loader, create a training set and validation set 
3. Dataset visualisation
-   Visualize one instance of all the class present in the dataset
-   Visualize distribution of classes in the training dataset
4. Class Imbalance: adding 500 samples per class to make sure that none of the classes are sparse
5. Model Building & training
-   Train the model on the data created using Augmentor.
-   Rescalling Layer - To rescale an input in the [0, 255] range to be in the [0, 1] range.
-   Choose an appropriate optimiser and loss function for model training
-   Train the model for ~20 epochs
-   Check if there is any evidence of model overfit or underfit.
## Overfitting
Using keras ImageDataGenerator to deal with Overfitting
## Conclusions
-   The class is imbalanced. Therefore, we should use Augmentor to rebalance data before the training model.
-   Use ImageDataGenerator to avoid overfitting
Initially, we tried building the model without the ImageDataGenerator which created data to highly overfit.

## Technologies Used
-   numpy
-   pandas
-   tensorflow
-   keras
-   matplotlib
-   seaborn
-   Augmentor
## Acknowledgements
-   Image Classification Using CNN - https://www.analyticsvidhya.com/blog/2020/02/learn-image-classification-cnn-convolutional-neural-networks-3-datasets/
-   Image Augmentation on the fly using Keras ImageDataGenerator! - https://www.analyticsvidhya.com/blog/2020/08/image-augmentation-on-the-fly-using-keras-imagedatagenerator/
-   Augmentor - https://augmentor.readthedocs.io/en/master/
## Contact
Created by Trang Le | github - @havu912