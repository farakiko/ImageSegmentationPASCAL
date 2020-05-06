# ImageSegmentationPASCAL
Image segmentation is a key problem in the field of computer vision with applications such as scene understanding, medical imaging, robot perception, image compression, augmented reality, and many others. Recently, deep learning has been proven success in a wide range of vision applications. In this project, we investigate the use of a fully convolutional network to solve over one of the most popular datasets used for semantic segmentation. The fully convolutional network under investigation is considered the state-of-the-art in image semantic segmentation.

## Dataset:
We will use the PASCAL VOC 2012 dataset for the segmentation task. The dataset is used for five different competitions: classification, detection, segmentation, action classification, and person layout. The images are ground-truth annotated and the dataset has 21 classes categorized into vehicles, household, animals, and others. This dataset is arguably one of most popular datasets for semantic segmentation and is divided into a training set of 1464 images, a validation set of 1449, and a testset.

## Objectives:
In this project, we will implement the FCN with VGG-16 as our base model. Our goal is to get adequate results compared to the results by Long et al, so we will set our baseline pixel accuracy to 83% (for the FCN-32s fixed). Transfer learning and fine-tuning will be considered in this task. In case the baseline wasn’t reached, we will implement the skip connection architecture and use different decoder pixel strides to enhance the results.

## References:
[1] https://arxiv.org/pdf/2001.05566.pdf
[2] Nameirakpam Dhanachandra et al “Image Segmentation Using K -means Clustering Algorithm and Subtractive Clustering Algorithm”
[3] Z. Huang and D. Liu, "Segmentation of Color Image Using EM algorithm in HSV Color Space," 2007 International Conference on Information Acquisition, Seogwipo-si, 2007, pp. 316-319.
[4] https://arxiv.org/abs/2001.05566
[5] https://arxiv.org/abs/1703.06870
[6] https://arxiv.org/pdf/1503.02351
[7] https://arxiv.org/pdf/1412.7062.pdf
[8] https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf


This Project was done by: Eslam Zaher & Farouk Mokhtar, at Zewail City of Science and Technology.
