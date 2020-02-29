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

last_modified_at: 2020-02-29T14:47:43+01:00
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
.tg  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-top-width:1px;border-bottom-width:1px;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-top-width:1px;border-bottom-width:1px;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-g1sy{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-8ot9{font-size:15px;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-zeup{background-color:#f9f9f9;font-style:italic;font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-8jvv{font-size:15px;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-yk9p{font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-z8x8{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-4dm3{font-size:15px;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-7xkh{background-color:#f9f9f9;font-style:italic;font-size:15px;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-dzk6{background-color:#f9f9f9;text-align:center;vertical-align:top}
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
    <td class="tg-yk9p" rowspan="8">Town 01, Hard Rain Noon, AudiTT<br>vs<br>Town 07, Hard Rain Noon, AudiTT</td>
    <td class="tg-g1sy" rowspan="4">AlexNet</td>
    <td class="tg-yk9p" rowspan="4">13,8627</td>
    <td class="tg-g1sy" rowspan="4">0,7135</td>
    <td class="tg-yk9p" rowspan="4">0,0295</td>
    <td class="tg-z8x8" rowspan="4">without<br>domain<br>adaptation </td>
    <td class="tg-4dm3">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf">[1]</a></td>
    <td class="tg-zeup"><span style="font-style:italic">(soon)</span></td>
    <td class="tg-yk9p">21,65</td>
  </tr>
  <tr>
    <td class="tg-4dm3">DeepLab V3+ <a href="https://eccv2018.org/openaccess/content_ECCV_2018/papers/Liang-Chieh_Chen_Encoder-Decoder_with_Atrous_ECCV_2018_paper.pdf">[2]</a></td>
    <td class="tg-zeup">(soon)</td>
    <td class="tg-yk9p">14,27</td>
  </tr>
  <tr>
    <td class="tg-4dm3">PSPNet <a href="http://openaccess.thecvf.com/content_cvpr_2017/papers/Zhao_Pyramid_Scene_Parsing_CVPR_2017_paper.pdf">[3]</a></td>
    <td class="tg-zeup">(soon)</td>
    <td class="tg-yk9p">14,64</td>
  </tr>
  <tr>
    <td class="tg-4dm3">PSANet <a href="https://link.springer.com/chapter/10.1007/978-3-030-01240-3_17">[4]</a></td>
    <td class="tg-zeup">(soon)</td>
    <td class="tg-yk9p">15,52</td>
  </tr>
  <tr>
    <td class="tg-g1sy" rowspan="4">ResNet-101</td>
    <td class="tg-yk9p" rowspan="4">6,6018</td>
    <td class="tg-g1sy" rowspan="4">1,0245</td>
    <td class="tg-yk9p" rowspan="4">0,0396</td>
    <td class="tg-z8x8" rowspan="4">with<br>domain<br>adaptation</td>
    <td class="tg-8jvv">DADA <a href="http://openaccess.thecvf.com/content_ICCV_2019/papers/Vu_DADA_Depth-Aware_Domain_Adaptation_in_Semantic_Segmentation_ICCV_2019_paper.pdf">[5]</a></td>
    <td class="tg-7xkh">(soon)</td>
    <td class="tg-8ot9">36,48</td>
  </tr>
  <tr>
    <td class="tg-0lax">ADVENT <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf">[6]</a></td>
    <td class="tg-dzk6"><span style="font-style:italic">(soon)</span></td>
    <td class="tg-baqh">39,30</td>
  </tr>
  <tr>
    <td class="tg-4dm3">CLAN <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf">[7]</a></td>
    <td class="tg-zeup">(soon)</td>
    <td class="tg-yk9p">41,18</td>
  </tr>
  <tr>
    <td class="tg-8jvv">DISE <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_All_About_Structure_Adapting_Structural_Information_Across_Domains_for_Boosting_CVPR_2019_paper.pdf">[8]</a></td>
    <td class="tg-7xkh">(soon)</td>
    <td class="tg-8ot9">46,71</td>
  </tr>
</table>