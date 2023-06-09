# CelebFaces

## Table of contents
* [Tasks](#tasks)
* [General info](#general-info)
* [Dataset info](#dataset-info)
* [Technologies](#technologies)
* [Source](#source)

## Tasks
Easy:
- Determining gender based on image analysis -> Gender.ipynb

Medium:
- Classification vs. image analysis (predicting a person's attractiveness based on image vs. predicting based on csv data) -> Attractiveness.ipynb 

Difficult:
- Face generator -> Face_generator.ipynb

## General info

![alt text](https://i.postimg.cc/5yp4715n/Celebrity.png)

Context:

A popular component of computer vision and deep learning revolves around identifying faces for various applications from logging into your phone with your face or searching through surveillance images for a particular suspect. This dataset is great for training and testing models for face detection, particularly for recognising facial attributes such as finding people with brown hair, are smiling, or wearing glasses. Images cover large pose variations, background clutter, diverse people, supported by a large quantity of images and rich annotations. This data was originally collected by researchers at MMLAB, The Chinese University of Hong Kong (specific reference in Acknowledgment section).

Overall:

- 202,599 number of face images of various celebrities
- 10,177 unique identities, but names of identities are not given
- 40 binary attribute annotations per image
- 5 landmark locations

## Dataset info
imgalignceleba.zip: All face images, cropped and aligned

listevalpartition.csv: Recommended partitioning of images into learning sets, validating, testing. Images 1-162770 are training, 162771-182637 are validation, 182638-202599 are testing

listbboxceleba.csv: envelope information for each image. "x1" and "y1" 
represent the coordinates of the upper left point of the bounding rectangle. "width" and "height" represent the width and height of the envelope

listlandmarksalign_celeba.csv: The image landmarks and their respective 
coordinates. There are 5 landmarks: left eye, right eye, nose, left mouth, 
right mouth

listattrceleba.csv: attribute labels for each image. There are 40 attributes. "1" indicates the presence of an attribute, and "-1" indicates the absence of an attribute

## Technologies
Project is created with:
* Python version: 3.10
* Keras verison: 2.12.0

## Source
https://www.kaggle.com/datasets/jessicali9530/celeba-dataset