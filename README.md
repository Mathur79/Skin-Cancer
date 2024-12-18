# SkinCancer

## Table of Contents
* [Problem Statement](#Problem-Statement)
* [Libraries Used](#Loading-Libraries)
* [Reading Datasets](#Reading-Datasets)
* [Data Preparation](#Data-Preparation)
* [View Images](#View-Images)
                                       
* [Model-1](#Model-1)
* [Model-1-Findings](#Model-1-Findings)
   
* [Model-2-DataAugumentation](#Model-2-DataAugumentation)
* [Model-2-DataAugumentation-Findings](#Model-2-DataAugumentation-Findings)

* [Rectify Class-Imbalance](#Class-Imbalance)

* [Model-3 (Post Class Imbalance)](#Model-3-(Post-Class-Imbalance))
* [Model-3 (Post-Class-Imbalance-Findings)](#Model-3(Post-Class-Imbalance-Findings))
* [Testing Validation](#Testing-Validation)
  
**Problem statement: 
**To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


**The data set contains the following diseases:**

Actinic keratosis

Basal cell carcinoma

Dermatofibroma

Melanoma

Nevus

Pigmented benign keratosis

Seborrheic keratosis

Squamous cell carcinoma


****Summary**

Model 1: (Using the Datasets as is)
The Model is Overfitting. There is huge difference between the Training and Validation Accuracy after 50 Epochs. Training Accuracy: 96% Validation Accuracy: 81%.

Model 2 (Augumentation).
The Model is no more Overfitting. The Accuracy Percentages in Training and Validation models are in the same range (same with the training and validation loss). Augumenting the data helped in mitigating the over fitting. However the overall accuracy is only 45% which is very low.

Model 3 (Addressed ClassImbalance)
Resolving the Class Imbalance helped resolve the overfitting to a large extent. Overfitting has also reduced given the difference is now 5%

Accuracy Percentages in Training : 91% Accuracy Percentage in Validation: 86%

