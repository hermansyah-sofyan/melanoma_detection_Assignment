# melanoma_detection_assignment
This is an assignment for MSc in Data Science. Collaboration courses between Upgrad, LJMU, and IIIT-Bengalore


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. This project is about Skin Cancer or Melanoma detection that is infered from various pictures of skin diseases. In order to do so, we need to build a CNN based model which can accurately detect melanoma.
Specifically, this is a solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

We processed 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- First iteration, we run using Convolutional and pooling only, we got an 0.94 accuracy for training, but only 0.80 for validation. So this indicated overfitting
- Second iteration, we run using dropouts, this improved the accuracy gap. With this method, we got 0.91 and 0.90 accuracy. But as we could see that there was imbalanced class, we still were able to increase the accuracy.
- Last iteration, we used augmentor to handle imbalanced class. After implementing this, we could increase the accuracy of training to 0.94 and validation accuracy 0.92. The accuracy gap was also considered small.
- For each CNN architecture, we included 3 different convolutional steps. First convolutional started with 16, 32, and then lastly 64 feature detectors with 3,3 kernels. On each convulutional, we implemented activation rectified linear activation function pool size 2,2 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
Tensorflow.keras version 2.12.0


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by Upgrad Assignment
- This project was based on [this tutorial](https://www.youtube.com/watch?v=jztwpsIzEGc).

## References
- Melanoma Skin Cancer from https://www.cancer.org/cancer/melanoma-skin-cancer/about/what-is-melanoma.html
- Introduction to CNN from https://www.analyticsvidhya.com/blog/2021/05/convolutional-neural-networks-cnn/
- Image classification using CNN from https://www.analyticsvidhya.com/blog/2020/02/learn-image-classification-cnn-convolutional-neural-networks-3-datasets/
- Convolutional Neural Network (CNN) for Automatic Skin Cancer Classification System from https://iopscience.iop.org/article/10.1088/1757-899X/982/1/012005/pdf

## Contact
Created by hermansyah1206@gmail.com - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
