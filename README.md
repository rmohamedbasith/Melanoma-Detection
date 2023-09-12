# Melanoma-Detection
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
-  Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion
  
**Solution Pipeline**
  - Data Reading/Data Understanding → Defining the path for train and test images 
  - Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
  - Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
  - Model Building & training : 
    - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
    - Choose an appropriate optimiser and loss function for model training
    - Train the model for epochs
  - Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
  - Model Building & training on the augmented data :
  - Class distribution: Examine the current class distribution in the training dataset 
  - Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.



## Conclusions
- Linear trend in both training and validation accuracy throughout the training process.
- As the number of training epochs increases, both training and validation accuracies exhibit consistent improvement. 
- The training loss is relatively low, indicating that the model is fitting the training data very well, with an accuracy of 89.67%.
- The validation loss is higher than the training loss, but the validation accuracy is still relatively high (83.69%).
Overall, these results suggest that the model is performing well and has a good balance between fitting the training data and generalizing to the validation data.


## Technologies Used
- tensorflow==2.12.0
- numpy==1.23.5
- pandas==1.5.3
- PIL==9.4.0
- keras.api._v2.keras==2.12.0
- Augmentor==0.2.12

## Contact
Created by [@MonikaDadhich] - feel free to contact me!
