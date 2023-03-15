# Early Stage Melanoma Detection using Deep Neural Network

### Introduction

Melanoma is a type of cancer that can deadly if it not detected early stage. Skin cancer causes 75% death due to this. 

### Problem Statement

We are trying to build such solution that system are able to idenfify the presense of Melanoma after processing image. So that It can aleart the respective 
dermatologists in early stage. It will also reduce potential manual work to idenfify the same.

We will build model which able to idenfiy one of category by processing image.

### Dataset Details:
1. This is open source image dataset which provided by International Skin Imaging Collaboration (ISIC).
2. Image has been taken by International Skin Imaging Collaboration (ISIC) with their specialized imaging equipments.
3. Dataset contains 2357 images having different 9 category classes.
4. The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

### Solution/Approaches:

I build CNN architecture and then I perfomred follwoing set of experiment.

1. verify CNN architecture with ablation experiment
2. ran model for few epoch with list of learning rate and found out stable learning rate to begin with.
3. trained model without augmentation of images for entire dataset. 
4. then train model with augmentation.
5. experiment with applying dropout, regularization.
