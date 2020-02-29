---
title: "IDDA vs IDDA"
layout: archive
toc: false
classes: wide
author_profile: false
read_time: false
comments: false
share: false
related: true

layouts_gallery_source:
  - url: /assets/images/viewpointchange_1/source1.jpg
    image_path: /assets/images/viewpointchange_1/source1.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/viewpointchange_1/source2.jpg
    image_path: /assets/images/viewpointchange_1/source2.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/viewpointchange_1/source3.jpg
    image_path: /assets/images/viewpointchange_1/source3.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/viewpointchange_1/source4.jpg
    image_path: /assets/images/viewpointchange_1/source4.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/viewpointchange_1/source5.jpg
    image_path: /assets/images/viewpointchange_1/source5.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/viewpointchange_1/source6.jpg
    image_path: /assets/images/viewpointchange_1/source6.jpg
    alt: "Source Example"
    title: "Source"
layouts_gallery_target:
  - url: /assets/images/viewpointchange_1/target1.jpg
    image_path: /assets/images/viewpointchange_1/target1.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/viewpointchange_1/target2.jpg
    image_path: /assets/images/viewpointchange_1/target2.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/viewpointchange_1/target3.jpg
    image_path: /assets/images/viewpointchange_1/target3.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/viewpointchange_1/target4.jpg
    image_path: /assets/images/viewpointchange_1/target4.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/viewpointchange_1/target5.jpg
    image_path: /assets/images/viewpointchange_1/target5.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/viewpointchange_1/target6.jpg
    image_path: /assets/images/viewpointchange_1/target6.jpg
    alt: "Target Example"
    title: "Target"
---
{% include feature_row id="intro" type="center" %}

## EXPERIMENT 1<br>Viewpoint Change
It tests the generalization and adaptation performances of the semantic segmentation networks when moving from a lower to an 
higher perspective, with a different shape of the hood.

### Source Scenario: 
- Environment: Town 01
- Weather and illumination condition: Clear Sunset
- Viewpoint: Audi TT
{% include gallery id="layouts_gallery_source" caption="Click to see some sample taken from the source scenario." %}

### Target/Test Scenario:
- Environment: Town 01
- Weather and illumination condition: Clear Sunset
- Viewpoint: Jeep Wrangler Rubicon
{% include gallery id="layouts_gallery_target" caption="Click to see some sample taken from the target/test scenario." %}

### Results
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-top-width:1px;border-bottom-width:1px;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-top-width:1px;border-bottom-width:1px;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-cly1{text-align:left;vertical-align:middle}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-9wq8{border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-buh4{background-color:#f9f9f9;text-align:left;vertical-align:top}
.tg .tg-nrix{text-align:center;vertical-align:middle}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-kyy7{background-color:#f9f9f9;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-dzk6{background-color:#f9f9f9;text-align:center;vertical-align:top}
.tg .tg-57iy{background-color:#f9f9f9;text-align:center;vertical-align:middle}
.tg .tg-d459{background-color:#f9f9f9;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-yjjc{background-color:#f9f9f9;text-align:left;vertical-align:middle}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-btxf{background-color:#f9f9f9;border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-nrix" rowspan="2">Experiment </th>
    <th class="tg-0lax" colspan="4">Distance</th>
    <th class="tg-0lax" colspan="4">Performance Evaluation</th>
  </tr>
  <tr>
    <td class="tg-buh4">Network</td>
    <td class="tg-9wq8">Euclidean</td>
    <td class="tg-kyy7">Cosine</td>
    <td class="tg-9wq8">Bhattacharaya</td>
    <td class="tg-dzk6" colspan="2">Network</td>
    <td class="tg-kyy7">Code Available</td>
    <td class="tg-9wq8">mIoU (%)</td>
  </tr>
  <tr>
    <td class="tg-9wq8" rowspan="8">Town 01, Clear Sunset, Audi TT<br>vs<br>Town 01, Clear Sunset, Jeep</td>
    <td class="tg-57iy" rowspan="4">AlexNet</td>
    <td class="tg-lboi" rowspan="4">5,6652</td>
    <td class="tg-d459" rowspan="4">0,1669</td>
    <td class="tg-lboi" rowspan="4">0,0155</td>
    <td class="tg-yjjc" rowspan="4">without<br>domain<br>adaptation </td>
    <td class="tg-lboi">DeepLab V2 [[]]()</td>
    <td class="tg-d459"><span style="font-style:italic">(soon)</span></td>
    <td class="tg-lboi">62,60</td>
  </tr>
  <tr>
    <td class="tg-lboi">DeepLab V3+ [[]]()</td>
    <td class="tg-d459">(soon)</td>
    <td class="tg-lboi">64,96</td>
  </tr>
  <tr>
    <td class="tg-lboi">PSPNet [[]]()</td>
    <td class="tg-d459">(soon)</td>
    <td class="tg-lboi">67,32</td>
  </tr>
  <tr>
    <td class="tg-lboi">PSANet [[]]()</td>
    <td class="tg-d459">(soon)</td>
    <td class="tg-lboi">66,88</td>
  </tr>
  <tr>
    <td class="tg-57iy" rowspan="4">ResNet-101</td>
    <td class="tg-cly1" rowspan="4">2,8014</td>
    <td class="tg-yjjc" rowspan="4">0,2937</td>
    <td class="tg-cly1" rowspan="4">0,0170</td>
    <td class="tg-yjjc" rowspan="4">with<br>domain<br>adaptation</td>
    <td class="tg-0lax">DADA [[]]()</td>
    <td class="tg-buh4">(soon)</td>
    <td class="tg-0lax">66,42</td>
  </tr>
  <tr>
    <td class="tg-0pky">ADVENT [[]]()</td>
    <td class="tg-btxf">(soon)</td>
    <td class="tg-0pky">68,43</td>
  </tr>
  <tr>
    <td class="tg-lboi">CLAN [[]]()</td>
    <td class="tg-d459">(soon)</td>
    <td class="tg-lboi">70,30</td>
  </tr>
  <tr>
    <td class="tg-0lax">DISE [[]]()</td>
    <td class="tg-buh4">(soon)</td>
    <td class="tg-0lax">73,64</td>
  </tr>
</table>