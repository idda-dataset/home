---
title: "Viewpoint Change"
layout: single
toc: false
classes: wide
author_profile: false
read_time: false
comments: false
share: false
related: false

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

last_modified_at: 2020-05-25T14:47:43+01:00
---
{% include feature_row id="intro" type="center" %}

## EXPERIMENT 1<br>From lower to higher viewpoint
It tests the generalization and adaptation performances of the semantic segmentation networks when moving from a lower to an 
higher perspective, with a different shape of the hood. The distance between the source and target scenario is low so, as a consequence, the task is easy. 

### Source Scenario: 
- Environment: Town 01
- Weather and illumination condition: Clear Sunset
- Viewpoint: Audi TT
- Source train set size: 10044
{% include gallery id="layouts_gallery_source" caption="Click to see some sample taken from the source scenario." %}

### Target/Test Scenario:
- Environment: Town 01
- Weather and illumination condition: Clear Sunset
- Viewpoint: Jeep Wrangler Rubicon
- Target train set size (only with DA): 10044
- Test size: 1674
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
    <td class="tg-lboi" rowspan="9"><span style="font-weight:bold">Source:</span><br>Town 01, Clear Sunset, Audi<br><br><span style="font-weight:bold">Target:</span><br>Town 01, Clear Sunset, Jeep</td>
    <td class="tg-z9fv" rowspan="9">6,4551</td>
    <td class="tg-lboi" rowspan="9">1,0586</td>
    <td class="tg-z9fv" rowspan="9">0,0426</td>
    <td class="tg-lboi" rowspan="5">without<br>domain<br>adaptation </td>
    <td class="tg-7d57">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf" target="_blank" rel="noopener noreferrer">[1]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">62,60</td>
  </tr>
  <tr>
    <td class="tg-7d57">DeepLab V3+ <a href="https://arxiv.org/pdf/1802.02611.pdf" target="_blank" rel="noopener noreferrer">[2]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">64,93</td>
  </tr>
  <tr>
    <td class="tg-7d57">PSPNet <a href="https://arxiv.org/abs/1612.01105" target="_blank" rel="noopener noreferrer">[3]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">67,32</td>
  </tr>
  <tr>
    <td class="tg-7d57">PSANet <a href="https://hszhao.github.io/papers/eccv18_psanet.pdf" target="_blank" rel="noopener noreferrer">[4]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">66,88</td>
  </tr>
  <tr>
    <td class="tg-dg7a">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf" target="_blank" rel="noopener noreferrer">[1]</a><br>(source=target)</td>
    <td class="tg-0lax">(soon)</td>
    <td class="tg-dg7a">79,13</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="4">with<br>domain<br>adaptation</td>
    <td class="tg-7d57">DADA <a href="http://openaccess.thecvf.com/content_ICCV_2019/papers/Vu_DADA_Depth-Aware_Domain_Adaptation_in_Semantic_Segmentation_ICCV_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[5]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">66,42</td>
  </tr>
  <tr>
    <td class="tg-7d57">ADVENT <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[6]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">68,43</td>
  </tr>
  <tr>
    <td class="tg-7d57">CLAN <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[7]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">70,30</td>
  </tr>
  <tr>
    <td class="tg-7d57">DISE <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_All_About_Structure_Adapting_Structural_Information_Across_Domains_for_Boosting_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[8]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">73,64</td>
  </tr>
</tbody>
</table>