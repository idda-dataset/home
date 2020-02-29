---
title: "IDDA vs BDD100K"
layout: archive
toc: false
classes: wide
author_profile: false
read_time: false
comments: false
share: false
related: true

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
  - url: /assets/images/iddavsbdd/target1.jpg
    image_path: /assets/images/iddavsbdd/target1.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsbdd/target2.jpg
    image_path: /assets/images/iddavsbdd/target2.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsbdd/target3.jpg
    image_path: /assets/images/iddavsbdd/target3.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsbdd/target4.jpg
    image_path: /assets/images/iddavsbdd/target4.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsbdd/target5.jpg
    image_path: /assets/images/iddavsbdd/target5.jpg
    alt: "Target Example"
    title: "Target"
  - url: /assets/images/iddavsbdd/target6.jpg
    image_path: /assets/images/iddavsbdd/target6.jpg
    alt: "Target Example"
    title: "Target"

last_modified_at: 2020-02-29T14:47:43+01:00
---
{% include feature_row id="intro" type="center" %}

## EXPERIMENT 1<br>From IDDA to BDD100K
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
- Environment: BDD100K
- Target train set size (only with DA): 3333
- Test size: 745
{% include gallery id="layouts_gallery_target" caption="Click to see some sample taken from the target/test scenario." %}

### Results
#### Best Case Scenario
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-top-width:1px;border-bottom-width:1px;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-top-width:1px;border-bottom-width:1px;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-g1sy{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-8ot9{font-size:15px;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-zeup{background-color:#f9f9f9;font-style:italic;font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-8jvv{font-size:15px;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-yk9p{font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-z8x8{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-4dm3{font-size:15px;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-7xkh{background-color:#f9f9f9;font-style:italic;font-size:15px;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-abip{background-color:#f9f9f9;border-color:inherit;text-align:center;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-yk9p" rowspan="2">Experiment </th>
    <th class="tg-8jvv" colspan="4">Distance</th>
    <th class="tg-8jvv" colspan="4">Performance Evaluation</th>
  </tr>
  <tr>
    <td class="tg-g1sy">Network</td>
    <td class="tg-yk9p">Euclidean<br>distance</td>
    <td class="tg-g1sy">Cosine<br>distance</td>
    <td class="tg-yk9p">Bhattacharaya<br>distance</td>
    <td class="tg-g1sy" colspan="2">Network</td>
    <td class="tg-g1sy">Code Available</td>
    <td class="tg-yk9p">mIoU (%)</td>
  </tr>
  <tr>
    <td class="tg-yk9p" rowspan="5">IDDA Best Case Scenario<br>vs<br>BDD100K </td>
    <td class="tg-g1sy">AlexNet</td>
    <td class="tg-yk9p">16,4401</td>
    <td class="tg-g1sy">1,4484</td>
    <td class="tg-yk9p">0,0216</td>
    <td class="tg-z8x8">without <br>domain <br>adaptation</td>
    <td class="tg-4dm3">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf">[1]</a></td>
    <td class="tg-zeup">(soon)</td>
    <td class="tg-yk9p">24,18</td>
  </tr>
  <tr>
    <td class="tg-g1sy" rowspan="4">ResNet-101</td>
    <td class="tg-yk9p" rowspan="4">5,8681</td>
    <td class="tg-g1sy" rowspan="4">14896</td>
    <td class="tg-yk9p" rowspan="4">0,0230</td>
    <td class="tg-z8x8" rowspan="4">with <br>domain<br>adaptation</td>
    <td class="tg-8jvv">DADA <a href="http://openaccess.thecvf.com/content_ICCV_2019/papers/Vu_DADA_Depth-Aware_Domain_Adaptation_in_Semantic_Segmentation_ICCV_2019_paper.pdf">[2]</a></td>
    <td class="tg-7xkh">(soon)</td>
    <td class="tg-8ot9">29,58</td>
  </tr>
  <tr>
    <td class="tg-0pky">ADVENT <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf">[3]</a></td>
    <td class="tg-abip">(soon)</td>
    <td class="tg-c3ow">33,18</td>
  </tr>
  <tr>
    <td class="tg-4dm3">CLAN <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf">[4]</a></td>
    <td class="tg-zeup">(soon)</td>
    <td class="tg-yk9p">33,47</td>
  </tr>
  <tr>
    <td class="tg-8jvv">DISE <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_All_About_Structure_Adapting_Structural_Information_Across_Domains_for_Boosting_CVPR_2019_paper.pdf">[5]</a></td>
    <td class="tg-7xkh">(soon)</td>
    <td class="tg-8ot9">40,09</td>
  </tr>
</table>

#### Worst Case Scenario
