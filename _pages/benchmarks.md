---
permalink: /benchmarks/
layout: single
toc: false
author_profile: false
title: "Benchmarks"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/benchmark.jpg
---
# IDDA vs IDDA
{% for post in site.IDDAvsIDDA limit: 5 %}
  {% include archive-single.html %}
{% endfor %}

# IDDA vs Real Dataset
{% for post in site.IDDAvsReal limit: 5 %}
  {% include archive-single.html %}
{% endfor %}

## The metric
### Performance evaluation
To evaluate the performances of the treated methods we use the PASCAL VOC Intersection-over-Union (IoU), also known 
as the Jaccard Index, that is essentially a method use to quantify the area of overlap divided by the area of union between 
the predicted segmentation and the ground truth. Quite simply, the IoU metric measure the number of pixels common between the target
and prediction masks and divide it by the total number of pixels
present across both masks (TP / (TP + FP + FN), where TP, FP and FN stands for True Positive, False Positive and False Negative 
respectively) [[1]](http://host.robots.ox.ac.uk/pascal/VOC/pubs/everingham15.pdf).
<br>The IoU is computed for each class separately and then averaged over all the classes to provide a global, mean IoU score 
(**mIoU**) for our semantic segmentation prediction. 
{: style="text-align: justify;"}

### Distance among domains 
To measure the distance and the similarity between two or more domains we proceed in this way: 
- for each domain, we randomly select 500 samples;
- for each sample, we extract the feature using an AlexNet [[2]](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf) 
and a ResNet-101 [[3]](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf);
- we reduce the dimensionality applying PCA and taking the first 50 principal components;
- we compute, in one case, the mean-feature vector for each domain and use it to measure the Euclidean and Cosine distance;
- we compute, in the other case, the feature-wise Bhattacharaya distance;
- additionally we use tSNE [[4]](http://www.jmlr.org/papers/volume9/vandermaaten08a/vandermaaten08a.pdf) to project the features extracted from the ResNet-101 in a more comprehensible 2D dimensional space.<br><br>
To reproduce our results we provide **here the code** both for the [[AlexNet]](https://github.com/taveraantonio/tSNE_AlexNet) and 
the [[ResNet-101]](https://github.com/taveraantonio/tSNE_ResNet) with the tSNE computation included.
{: style="text-align: justify;"}


This section and all of its subsections will be constantly updated as soon as new benchmarks will be performed. 
<br>To whoever wants to submit its results will be soon deployed a dedicated page.
{: .notice--info}