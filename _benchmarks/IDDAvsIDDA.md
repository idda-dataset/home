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
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-9wq8{border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-baqh" rowspan="2"><br>Experiment </th>
    <th class="tg-baqh" colspan="3">Distance</th>
    <th class="tg-baqh" colspan="3">Performance evaluation</th>
  </tr>
  <tr>
    <td class="tg-9wq8">Euclidean</td>
    <td class="tg-9wq8">Cosine</td>
    <td class="tg-9wq8">Bhattacharaya</td>
    <td class="tg-9wq8">Network</td>
    <td class="tg-9wq8">Code Available</td>
    <td class="tg-9wq8">mIoU</td>
  </tr>
  <tr>
    <td class="tg-9wq8" rowspan="6">Town 01, Clear Sunset, Audi TT<br>vs<br>Town 01, Clear Sunset, Jeep</td>
    <td class="tg-lboi" rowspan="6"></td>
    <td class="tg-lboi" rowspan="6"></td>
    <td class="tg-lboi" rowspan="6"></td>
    <td class="tg-lboi">DeepLab V2</td>
    <td class="tg-lboi"></td>
    <td class="tg-lboi"></td>
  </tr>
  <tr>
    <td class="tg-lboi">DeepLab V3+</td>
    <td class="tg-lboi"></td>
    <td class="tg-lboi"></td>
  </tr>
  <tr>
    <td class="tg-lboi">PSPNet</td>
    <td class="tg-lboi"></td>
    <td class="tg-lboi"></td>
  </tr>
  <tr>
    <td class="tg-lboi">PSANet</td>
    <td class="tg-lboi"></td>
    <td class="tg-lboi"></td>
  </tr>
  <tr>
    <td class="tg-0pky">DISE</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-lboi"></td>
    <td class="tg-lboi"></td>
    <td class="tg-lboi"></td>
  </tr>
</table>