---
title: "Town Change"
layout: single
toc: false
classes: wide
author_profile: false
read_time: false
comments: false
share: false
related: false

layouts_gallery_source:
  - url: /assets/images/townchange_2/source1.jpg
    image_path: /assets/images/townchange_2/source1.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/townchange_2/source2.jpg
    image_path: /assets/images/townchange_2/source2.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/townchange_2/source3.jpg
    image_path: /assets/images/townchange_2/source3.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/townchange_2/source4.jpg
    image_path: /assets/images/townchange_2/source4.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/townchange_2/source5.jpg
    image_path: /assets/images/townchange_2/source5.jpg
    alt: "Source Example"
    title: "Source"
  - url: /assets/images/townchange_2/source6.jpg
    image_path: /assets/images/townchange_2/source6.jpg
    alt: "Source Example"
    title: "Source"
layouts_gallery_target:
  - url: /assets/images/townchange_2/target1.jpg
    image_path: /assets/images/townchange_2/target1.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/townchange_2/target2.jpg
    image_path: /assets/images/townchange_2/target2.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/townchange_2/target3.jpg
    image_path: /assets/images/townchange_2/target3.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/townchange_2/target4.jpg
    image_path: /assets/images/townchange_2/target4.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/townchange_2/target5.jpg
    image_path: /assets/images/townchange_2/target5.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/townchange_2/target6.jpg
    image_path: /assets/images/townchange_2/target6.jpg
    alt: "Target Example"
    title: "Target"

last_modified_at: 2020-05-25T14:47:43+01:00
---
{% include feature_row id="intro" type="center" %}

## EXPERIMENT 2<br>From a city to a bucolic country
It tests the generalization and adaptation performances of the semantic segmentation networks when changing completely the environment, 
moving from a city to a countryside. The distance between the source and target scenario is high so, as a consequence, the task is difficult. 
The task is even more challenging due to the rain condition.

### Source Scenario: 
- Environment: Town 01
- Weather and illumination condition: Hard Rain Noon
- Viewpoint: Audi TT
- Source train set size: 10008
{% include gallery id="layouts_gallery_source" caption="Click to see some sample taken from the source scenario." %}

### Target/Test Scenario:
- Environment: Town 07
- Weather and illumination condition: Hard Rain Noon
- Viewpoint: Audi TT
- Target train set size (only with DA): 10008
- Test size: 1672
{% include gallery id="layouts_gallery_target" caption="Click to see some sample taken from the target/test scenario." %}

### Results
<style type="text/css">
.tg  {border:none;border-collapse:collapse;border-color:#aaa;border-spacing:0;}
.tg td{background-color:#fff;border-color:#aaa;border-style:solid;border-width:0px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#f38630;border-color:#aaa;border-style:solid;border-width:0px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-7d57{background-color:#FCFBE3;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-z9fv{background-color:#FCFBE3;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-dg7a{background-color:#FCFBE3;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow" rowspan="2">Experiment </th>
    <th class="tg-c3ow" colspan="3">Distance Measurement</th>
    <th class="tg-c3ow" colspan="4">Performance Evaluation</th>
  </tr>
  <tr>
    <td class="tg-7d57">Euclidean<br>distance</td>
    <td class="tg-0pky">Cosine<br>distance</td>
    <td class="tg-7d57">Bhattacharaya<br>distance</td>
    <td class="tg-c3ow" colspan="2">Network</td>
    <td class="tg-0pky">Code Available</td>
    <td class="tg-7d57">mIoU (%)</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-lboi" rowspan="9"><span style="font-weight:bold">Source:</span><br>Town 01, Hard Rain Noon, Audi<br><br><span style="font-weight:bold">Target:</span><br>Town 07, Hard Rain Noon, Audi</td>
    <td class="tg-z9fv" rowspan="9">6,4551</td>
    <td class="tg-lboi" rowspan="9">1,0586</td>
    <td class="tg-z9fv" rowspan="9">0,0426</td>
    <td class="tg-lboi" rowspan="5">without<br>domain<br>adaptation </td>
    <td class="tg-7d57">DeepLab V2 [1]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">21,65</td>
  </tr>
  <tr>
    <td class="tg-7d57">DeepLab V3+ [2]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">14,27</td>
  </tr>
  <tr>
    <td class="tg-7d57">PSPNet [3]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">14,64</td>
  </tr>
  <tr>
    <td class="tg-7d57">PSANet [4]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">15,52</td>
  </tr>
  <tr>
    <td class="tg-dg7a">DeepLab V2 [1]<br>(source=target)</td>
    <td class="tg-0lax">(soon)</td>
    <td class="tg-dg7a">78,02</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="4">with<br>domain<br>adaptation</td>
    <td class="tg-7d57">DADA [5]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">36,48</td>
  </tr>
  <tr>
    <td class="tg-7d57">ADVENT [6]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">39,30</td>
  </tr>
  <tr>
    <td class="tg-7d57">CLAN [7]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">41,18</td>
  </tr>
  <tr>
    <td class="tg-7d57">DISE [8]</td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">46,71</td>
  </tr>
</tbody>
</table>