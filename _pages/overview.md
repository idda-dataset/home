---
permalink: /overview/
layout: splash
toc: false
author_profile: false
title: "Overview"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/overview2.jpg

layouts_gallery:
  - url: /assets/images/RGB.jpg
    image_path: /assets/images/RGB.jpg
    alt: "RGB Image Example"
  - url: /assets/images/Semantic.jpg
    image_path: /assets/images/Semantic.jpg
    alt: "Semantic Image Example"
  - url: /assets/images/Depth.jpg
    image_path: /assets/images/Depth.jpg
    alt: "Depth Image Example"
last_modified_at: 2020-02-26T11:23:43+01:00
---


## Notable features
### Type of data: 
- RGB
- Pixel-wise Semantic annotation
- Depth maps
- Semantic-RGB Cityscapes-palette conversion
- Depth Gray-scale
- Logarithmic Depth Gray-scale

### Dataset Dimensions: 
- 1,006,800 images for each data type
- 1920x1080 pixels
- FoV of 90°
- 4TB of memory usage

### Data Diversity: 
- 6 cities + 1 bucolic country 
- 3 weather and illumination conditions:
  - Clear Noon
  - Clear Sunset
  - Hard Rain Noon
- 5 different camera heights (from lower to higher position)
- 5 viewpoints with and without hood (if visible, hood different in shape and color)
- 105 different scenarios with around 16k training/testing images for each
- Distributions of vehicles and pedestrians in the scene always changing

## Semantic Segmentation
- 24 semantic classes
- 2087.70 x 10<sup>9</sup> annotated pixels
### Classes Description:
| Class Number 	| Name 	| Description 	|
|--------------	|------	|-------------	|
| 0            	|      	|             	|
| 1            	|      	|             	|
| 2            	|      	|             	|
| 3            	|      	|             	|
| 4            	|      	|             	|
| 5            	|      	|             	|
| 6            	|      	|             	|
| 7            	|      	|             	|
| 8            	|      	|             	|
| 9            	|      	|             	|
| 10           	|      	|             	|
| 11           	|      	|             	|
| 12           	|      	|             	|
| 13           	|      	|             	|
| 14           	|      	|             	|
| 15           	|      	|             	|
| 16           	|      	|             	|
| 17           	|      	|             	|
| 18           	|      	|             	|
| 19           	|      	|             	|
| 20           	|      	|             	|
| 21           	|      	|             	|
| 22           	|      	|             	|
| 23           	|      	|             	|



{% include gallery id="layouts_gallery" caption="Click to see some sample taken from IDDA:`RGB`, `Semantic`, and `Depth`." %}

