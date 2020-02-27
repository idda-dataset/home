---
permalink: /overview/
layout: single
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
    title: "RGB Image Example"
  - url: /assets/images/Semantic.jpg
    image_path: /assets/images/Semantic.jpg
    alt: "Semantic Image Example"
    title: "Semantic Image Example"
  - url: /assets/images/Depth.jpg
    image_path: /assets/images/Depth.jpg
    alt: "Depth Image Example"
    title: "Depth Image Example"
  
last_modified_at: 2020-02-26T11:23:43+01:00
---


## Notable features
### Type of data: 
- RGB
- Pixel-wise Semantic annotation
- Depth map
- Semantic RGB Cityscapes-palette conversion
- Depth Gray-scale
- Logarithmic Depth Gray-scale

### Dataset Dimensions: 
- 1,006,800 images for each data type
- 1920x1080 pixels
- FoV of 90°
- 4TB of memory occupation

### Data Diversity: 
- 6 cities + 1 bucolic country 
- 3 weather and illumination conditions:
  - Clear Noon
  - Clear Sunset
  - Hard Rain Noon
- 5 different camera heights (from lower to higher position)
- 5 viewpoints with and without hood (if visible, hood different in shape and color):
  - Audi TT
  - Ford Mustang
  - Jeep Wrangler Rubicon
  - Volkswagen T2
  - Bus  
- 105 different scenarios with around 16k training/testing images for each
- Always different distributions of vehicles and pedestrians in the scenes

## Semantic Segmentation
- 24 semantic classes
- 2087.70 x 10<sup>9</sup> annotated pixels
### Classes Definition:

    | Class | Name          | Description                                                                             |
    |-------|---------------|-----------------------------------------------------------------------------------------|
    | 0*    | None          | all the remaining objects not labeled                                              |
    | 1     | Building      | skyscraper, house, bust stop, garage, bridge,fountains and other types of constructions |
    | 2     | Fence         | barrier, railing or other upright structure                                             |
    | 3*    | Other         | all static objects not classified, but not None                                         |
    | 4     | Pedestrian    | human person (male, female or kids). Not included what is carried by the person         |
    | 5     | Pole          | vertical oriented piece of wood or metal                                                |
    | 6*    | Road line     | all the marks on the road, line painted on the pavements                                |
    | 7     | Road          | any kind of drivable road                                                               |
    | 8     | Sidewalk      | part of the ground designated only for pedestrian                                       |
    | 9     | Vegetation    | tree, hedge, plants                                                                     |
    | 10    | Vehicles      | cars and truck, visible hood                                                            |
    | 11    | Wall          | vertical brick or stone structure                                                       |
    | 12    | Traffic Sign  | the part of the sign containing the information, not the pole                           |
    | 13    | Traffic Light | the traffic light box, without pole                                                     |
    | 14*   | Guardrail     | crash barriers                                                                          |
    | 15*   | Dynamic       | movable objects like trash, bin, bag or wheelchair                                      |
    | 16    | Bicycle       | cross bikes, leisures bike and road bikes                                               |
    | 17    | Motorcycle    | four kind of motorbikes                                                                 |
    | 18    | Rider         | rider of bike or motorcycle, not pedestrian                                             |
    | 19    | Terrain       | background, grass, soil, sand or rocks                                                  |
    | 20    | Sky           | the open sky                                                                            |
    | 21*   | Railway       | rail truck or elevated rail line                                                        |
    | 22*   | Ground        | horizontal ground-level structure                                                       |
    | 23*   | Static        | clutter in the background not distinguishable, like mountains                           |
    
    *This class is not considered during evaluation
    {: .notice}
    
    
{% include gallery id="layouts_gallery" caption="Click to see some sample taken from IDDA:`RGB`, `Semantic`, and `Depth`." %}

