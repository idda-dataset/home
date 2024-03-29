---
title: "IDDA vs A2D2"
layout: single
toc: false
classes: wide
author_profile: false
read_time: false
comments: false
share: false
related: false

layouts_gallery_best:
  - url: /assets/images/iddavsbdd/source_best1.jpg
    image_path: /assets/images/iddavsbdd/source_best1.jpg
    alt: "Source Best Example"
    title: "Source Best"
  - url: /assets/images/iddavsbdd/source_best2.jpg
    image_path: /assets/images/iddavsbdd/source_best2.jpg
    alt: "Source Best Example"
    title: "Source Best"
  - url: /assets/images/iddavsbdd/source_best3.jpg
    image_path: /assets/images/iddavsbdd/source_best3.jpg
    alt: "Source Example"
    title: "Source Best"
  - url: /assets/images/iddavsbdd/source_best4.jpg
    image_path: /assets/images/iddavsbdd/source_best4.jpg
    alt: "Source Example"
    title: "Source Best"
  - url: /assets/images/iddavsbdd/source_best5.jpg
    image_path: /assets/images/iddavsbdd/source_best5.jpg
    alt: "Source Example"
    title: "Source Best"
  - url: /assets/images/iddavsbdd/source_best6.jpg
    image_path: /assets/images/iddavsbdd/source_best6.jpg
    alt: "Source Example"
    title: "Source Best"
layouts_gallery_worst:
  - url: /assets/images/iddavsbdd/source_worst1.jpg
    image_path: /assets/images/iddavsbdd/source_worst1.jpg
    alt: "Source Worst Example"
    title: "Source Worst"
  - url: /assets/images/iddavsbdd/source_worst2.jpg
    image_path: /assets/images/iddavsbdd/source_worst2.jpg
    alt: "Source Worst Example"
    title: "Source Worst"
  - url: /assets/images/iddavsbdd/source_worst3.jpg
    image_path: /assets/images/iddavsbdd/source_worst3.jpg
    alt: "Source Worst Example"
    title: "Source Worst"
  - url: /assets/images/iddavsbdd/source_worst4.jpg
    image_path: /assets/images/iddavsbdd/source_worst4.jpg
    alt: "Source Worst Example"
    title: "Source Worst"
  - url: /assets/images/iddavsbdd/source_worst5.jpg
    image_path: /assets/images/iddavsbdd/source_worst5.jpg
    alt: "Source Worst Example"
    title: "Source Worst"
  - url: /assets/images/iddavsbdd/source_worst6.jpg
    image_path: /assets/images/iddavsbdd/source_worst6.jpg
    alt: "Source Worst Example"
    title: "Source Worst"
layouts_gallery_target:
  - url: /assets/images/iddavsa2d2/target1.jpg
    image_path: /assets/images/iddavsa2d2/target1.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsa2d2/target2.jpg
    image_path: /assets/images/iddavsa2d2/target2.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsa2d2/target3.jpg
    image_path: /assets/images/iddavsa2d2/target3.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsa2d2/target4.jpg
    image_path: /assets/images/iddavsa2d2/target4.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsa2d2/target5.jpg
    image_path: /assets/images/iddavsa2d2/target5.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsa2d2/target6.jpg
    image_path: /assets/images/iddavsa2d2/target6.jpg
    alt: "Target Example"
    title: "Target"

last_modified_at: 2020-05-25T14:47:43+01:00
---
{% include feature_row id="intro" type="center" %}

## EXPERIMENT 4<br>From IDDA to A2D2
It tests how well the networks trained with images taken from the synthetic world adapt to the real one and how the different distribution 
of data in IDDA affect the performance in the real target domain. To do so, we repeated the experiment two times considering as source domain 
two different IDDA distributions, one more similar and close to the real dataset (best case), the other much more different and faraway (worst case).


### Source Scenario: 
#### Best case scenario
- Environment: Town 01, 02, 03, 04, 05, 06
- Weather and illumination condition: Clear Noon
- Viewpoint: Audi TT, Ford Mustang
- Source train set size: 29952
{% include gallery id="layouts_gallery_best" caption="Click to see some sample taken from the best source scenario." %}
#### Worst case scenario
- Environment: Town 07
- Weather and illumination condition: Hard Rain Noon
- Viewpoint: Jeep Wrangler(with hood), Bus(without hood)
- Source train set size: 40128
{% include gallery id="layouts_gallery_worst" caption="Click to see some sample taken from the worst source scenario." %}

### Target/Test Scenario:
- Dataset: Audi Driving Dataset - A2D2
- Environment: three different German cities 
- Weather and illumination condition: various
- Viewpoints: camera front center
- Target train set size (only with domain adaptation): 18878
- Test size: 3147
{% include gallery id="layouts_gallery_target" caption="Click to see some sample taken from the target/test scenario." %}



### Results
#### Best Case Scenario
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#aaa;border-spacing:0;}
.tg td{background-color:#fff;border-bottom-width:1px;border-color:#aaa;border-style:solid;border-top-width:1px;
  border-width:0px;color:#333;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;
  word-break:normal;}
.tg th{background-color:#f38630;border-bottom-width:1px;border-color:#aaa;border-style:solid;border-top-width:1px;
  border-width:0px;color:#fff;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;
  padding:10px 5px;word-break:normal;}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-7d57{background-color:#FCFBE3;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-z9fv{background-color:#FCFBE3;border-color:inherit;text-align:left;vertical-align:middle}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky" rowspan="2">Experiment </th>
    <th class="tg-c3ow" colspan="3">Distance Measurements</th>
    <th class="tg-c3ow" colspan="4">Performance Evaluation</th>
  </tr>
  <tr>
    <td class="tg-7d57">Euclidean<br>distance</td>
    <td class="tg-0pky">Cosine<br>distance</td>
    <td class="tg-7d57">Bhattacharaya<br>distance</td>
    <td class="tg-0pky" colspan="2">Network</td>
    <td class="tg-0pky">Code Available</td>
    <td class="tg-7d57">mIoU (%)</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-lboi" rowspan="5"><span style="font-weight:bold">Source:</span><br>IDDA Best Case <br><br><span style="font-weight:bold">Target:</span><br>A2D2*</td>
    <td class="tg-z9fv" rowspan="5">6,3874</td>
    <td class="tg-lboi" rowspan="5">1,0589</td>
    <td class="tg-z9fv" rowspan="5">0,0447</td>
    <td class="tg-0pky">without <br>domain <br>adaptation</td>
    <td class="tg-7d57">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf" target="_blank" rel="noopener noreferrer">[1]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">32,10</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="4">with <br>domain<br>adaptation</td>
    <td class="tg-7d57">DADA <a href="http://openaccess.thecvf.com/content_ICCV_2019/papers/Vu_DADA_Depth-Aware_Domain_Adaptation_in_Semantic_Segmentation_ICCV_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[2]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">38,57</td>
  </tr>
  <tr>
    <td class="tg-7d57">ADVENT <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[3]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">42,56</td>
  </tr>
  <tr>
    <td class="tg-7d57">CLAN <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[4]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">44,31</td>
  </tr>
  <tr>
    <td class="tg-7d57">DISE <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_All_About_Structure_Adapting_Structural_Information_Across_Domains_for_Boosting_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[5]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">46,73</td>
  </tr>
</tbody>
</table>

#### Worst Case Scenario
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#aaa;border-spacing:0;}
.tg td{background-color:#fff;border-bottom-width:1px;border-color:#aaa;border-style:solid;border-top-width:1px;
  border-width:0px;color:#333;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;
  word-break:normal;}
.tg th{background-color:#f38630;border-bottom-width:1px;border-color:#aaa;border-style:solid;border-top-width:1px;
  border-width:0px;color:#fff;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;
  padding:10px 5px;word-break:normal;}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-7d57{background-color:#FCFBE3;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-z9fv{background-color:#FCFBE3;border-color:inherit;text-align:left;vertical-align:middle}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky" rowspan="2">Experiment </th>
    <th class="tg-c3ow" colspan="3">Distance Measurements</th>
    <th class="tg-c3ow" colspan="4">Performance Evaluation</th>
  </tr>
  <tr>
    <td class="tg-7d57">Euclidean<br>distance</td>
    <td class="tg-0pky">Cosine<br>distance</td>
    <td class="tg-7d57">Bhattacharaya<br>distance</td>
    <td class="tg-0pky" colspan="2">Network</td>
    <td class="tg-0pky">Code Available</td>
    <td class="tg-7d57">mIoU (%)</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-lboi" rowspan="5"><span style="font-weight:bold">Source:</span><br>IDDA Worst Case <br><br><span style="font-weight:bold">Target:</span><br>A2D2*</td>
    <td class="tg-z9fv" rowspan="5">7,0150</td>
    <td class="tg-lboi" rowspan="5">1,1849</td>
    <td class="tg-z9fv" rowspan="5">0,0387</td>
    <td class="tg-0pky">without <br>domain <br>adaptation</td>
    <td class="tg-7d57">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf" target="_blank" rel="noopener noreferrer">[1]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">29,80</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="4">with <br>domain<br>adaptation</td>
    <td class="tg-7d57">DADA <a href="http://openaccess.thecvf.com/content_ICCV_2019/papers/Vu_DADA_Depth-Aware_Domain_Adaptation_in_Semantic_Segmentation_ICCV_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[2]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">36,18</td>
  </tr>
  <tr>
    <td class="tg-7d57">ADVENT <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[3]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">38,57</td>
  </tr>
  <tr>
    <td class="tg-7d57">CLAN <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[4]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">42,71</td>
  </tr>
  <tr>
    <td class="tg-7d57">DISE <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_All_About_Structure_Adapting_Structural_Information_Across_Domains_for_Boosting_CVPR_2019_paper.pdf" target="_blank" rel="noopener noreferrer">[5]</a></td>
    <td class="tg-0pky">(soon)</td>
    <td class="tg-7d57">45,49</td>
  </tr>
</tbody>
</table>

*The number of classes considered during evaluation is 13 (w.r.t. to the other experiments where 16 classes in common
between IDDA and the other real-world dataset are chosen).
{: .notice--warning}
