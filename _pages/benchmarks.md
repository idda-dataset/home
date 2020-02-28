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

{% for post in site.benchmarks limit: 5 %}
  {% include archive-single.html %}
{% endfor %}

{% include feature_row id="intro" type="center" %}

## The metric

### Performance evaluation
To evaluate the performances of the treated methods we use the PASCAL VOC Intersection-over-Union (IoU), also known 
as the Jaccard Index, that is essentially a method use to quantify the area of overlap between the predicted segmentation 
and the ground truth divided by the area of union between the predicted segmentation and the ground truth. Quite simply, the IoU 
metric measure the number of pixels common between the target and prediction masks and divide it by the total number of pixels
present across both masks (TP / (TP + FP + FN), where TP, FP and FN stands for True Positive, False Positive and False Negative 
respectively)[[1]](http://host.robots.ox.ac.uk/pascal/VOC/pubs/everingham15.pdf).
<br>The IoU is computed for each class eparately and the averaged over all the classes to provide a gloabal, mean Iou score 
(**mIoU**) for our semantic segmentation prediction. 
{: style="text-align: justify;"}

### Distance among domains 
