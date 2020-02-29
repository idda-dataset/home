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

layouts_gallery1:
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

---
{% include feature_row id="intro" type="center" %}

## EXPERIMENT 1<br>Viewpoint Change

### Source Scenario: 
Town 01, Clear Sunset, Audi TT
{% include gallery id="layouts_gallery1" caption="Click to see some sample taken from the source scenario." %}

### Target/Test Scenario:<br>Town01, Clear Sunset, Jeep Wrangler Rubicon
{% include gallery id="layouts_gallery1" caption="Click to see some sample taken from the target/test scenario." %}

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