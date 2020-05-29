# ImageSegmentationPASCAL

The main goal of this work is to recognize objects from a number of visual object classes through the generation of a visually segmented picture of the input image. It is  a supervised learning learning problem in that a training set of labelled images is provided. The twenty object classes that have been selected are:
- Person: person
- Animal: bird, cat, cow, dog, horse, sheep
- Vehicle: aeroplane, bicycle, boat, bus, car, motorbike, train
- Indoor: bottle, chair, dining table, potted plant, sofa, tv/monitor

In total, we have 21 classes including the background null class.

Simply put, our goal is to take an RGB color image (height×width×3) and output a segmentation map (height×width×1) where each pixel contains a class label represented as an integer. The following is a nice illustration of a segmentation problem:

![example](/images/example.jpg)

## Dataset:
We will use the PASCAL VOC 2012 dataset for the segmentation task. The dataset is used for five different competitions: classification, detection, segmentation, action classification, and person layout. The images are ground-truth annotated and the dataset has 21 classes categorized into vehicles, household, animals, and others. This dataset is arguably one of most popular datasets for semantic segmentation and is divided into a training set of 1464 images, a validation set of 1449, and a testset.

The data is obtained from the following reference: \
@misc{pascal-voc-2012,
author = "Everingham, M. and Van~Gool, L. and Williams, C. K. I. and Winn, J. and Zisserman, A.",
title = "The {PASCAL} {V}isual {O}bject {C}lasses {C}hallenge 2012 {(VOC2012)} {R}esults",
howpublished = "http://www.pascal-network.org/challenges/VOC/voc2012/workshop/index.html"}

## Our Model:
In this project, we will implement the FCN with VGG-16 as our base model. Our goal is to get adequate results compared to the results by Long et al, so we will set our baseline pixel accuracy to 83% (for the FCN-32s fixed). Transfer learning and fine-tuning will be considered in this task. In case the baseline wasn’t reached, we will implement the skip connection architecture and use different decoder pixel strides to enhance the results.

## Results:
We achieve a validation accuracy of 80%, which is comparable to the 83% validation accuracy achieved by Long et. al[8] given our resources.

## References:
[1] https://arxiv.org/pdf/2001.05566.pdf
[2] Nameirakpam Dhanachandra et al “Image Segmentation Using K -means Clustering Algorithm and Subtractive Clustering Algorithm”
[3] Z. Huang and D. Liu, "Segmentation of Color Image Using EM algorithm in HSV Color Space," 2007 International Conference on Information Acquisition, Seogwipo-si, 2007, pp. 316-319.
[4] https://arxiv.org/abs/2001.05566
[5] https://arxiv.org/abs/1703.06870
[6] https://arxiv.org/pdf/1503.02351
[7] https://arxiv.org/pdf/1412.7062.pdf
[8] Long at al. “Fully Convolutional Networks for Semantic Segmentation”



__This Project was done by: Eslam Zaher & Farouk Mokhtar, at Zewail City of Science and Technology.__
