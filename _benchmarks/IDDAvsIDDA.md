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
higher perspective, with a different shape of the hood. The distance between the source and target scenario is low. 

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
.tg .tg-76ut{background-color:#f9f9f9;font-size:15px;text-align:center;vertical-align:middle}
.tg .tg-oiyu{font-size:15px;text-align:left;vertical-align:middle}
.tg .tg-g1sy{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-8jvv{font-size:15px;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-iml5{background-color:#f9f9f9;font-size:15px;text-align:left;vertical-align:top}
.tg .tg-bg24{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-gmdn{background-color:#f9f9f9;font-size:15px;text-align:center;vertical-align:top}
.tg .tg-8goc{font-size:15px;text-align:center;vertical-align:middle}
.tg .tg-cbs6{font-size:15px;text-align:left;vertical-align:top}
.tg .tg-yk9p{font-size:15px;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-4dm3{font-size:15px;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-z8x8{background-color:#f9f9f9;font-size:15px;border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-2uvt{background-color:#f9f9f9;font-size:15px;text-align:left;vertical-align:middle}
.tg .tg-vncu{font-size:15px;font-family:serif !important;;border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-8goc" rowspan="2">Experiment </th>
    <th class="tg-cbs6" colspan="4">Distance</th>
    <th class="tg-cbs6" colspan="4">Performance Evaluation</th>
  </tr>
  <tr>
    <td class="tg-iml5">Network</td>
    <td class="tg-yk9p">Euclidean</td>
    <td class="tg-g1sy">Cosine</td>
    <td class="tg-yk9p">Bhattacharaya</td>
    <td class="tg-gmdn" colspan="2">Network</td>
    <td class="tg-g1sy">Code Available</td>
    <td class="tg-yk9p">mIoU (%)</td>
  </tr>
  <tr>
    <td class="tg-yk9p" rowspan="8">Town 01, Clear Sunset, Audi TT<br>vs<br>Town 01, Clear Sunset, Jeep</td>
    <td class="tg-76ut" rowspan="4">AlexNet</td>
    <td class="tg-4dm3" rowspan="4">5,6652</td>
    <td class="tg-z8x8" rowspan="4">0,1669</td>
    <td class="tg-4dm3" rowspan="4">0,0155</td>
    <td class="tg-2uvt" rowspan="4">without<br>domain<br>adaptation </td>
    <td class="tg-4dm3">DeepLab V2 <a href="https://arxiv.org/pdf/1606.00915.pdf">[1]</a></td>
    <td class="tg-z8x8"><span style="font-style:italic">(soon)</span></td>
    <td class="tg-4dm3">62,60</td>
  </tr>
  <tr>
    <td class="tg-4dm3">DeepLab V3+ <a href="https://eccv2018.org/openaccess/content_ECCV_2018/papers/Liang-Chieh_Chen_Encoder-Decoder_with_Atrous_ECCV_2018_paper.pdf">[2]</a></td>
    <td class="tg-z8x8">(soon)</td>
    <td class="tg-4dm3">64,96</td>
  </tr>
  <tr>
    <td class="tg-4dm3">PSPNet <a href="http://openaccess.thecvf.com/content_cvpr_2017/papers/Zhao_Pyramid_Scene_Parsing_CVPR_2017_paper.pdf">[3]</a></td>
    <td class="tg-z8x8">(soon)</td>
    <td class="tg-4dm3">67,32</td>
  </tr>
  <tr>
    <td class="tg-4dm3">PSANet <a href="https://link.springer.com/chapter/10.1007/978-3-030-01240-3_17">[4]</a></td>
    <td class="tg-z8x8">(soon)</td>
    <td class="tg-4dm3">66,88</td>
  </tr>
  <tr>
    <td class="tg-76ut" rowspan="4">ResNet-101</td>
    <td class="tg-oiyu" rowspan="4">2,8014</td>
    <td class="tg-2uvt" rowspan="4">0,2937</td>
    <td class="tg-oiyu" rowspan="4">0,0170</td>
    <td class="tg-2uvt" rowspan="4">with<br>domain<br>adaptation</td>
    <td class="tg-cbs6">DADA <a href="http://openaccess.thecvf.com/content_ICCV_2019/papers/Vu_DADA_Depth-Aware_Domain_Adaptation_in_Semantic_Segmentation_ICCV_2019_paper.pdf">[5]</a></td>
    <td class="tg-iml5">(soon)</td>
    <td class="tg-cbs6">66,42</td>
  </tr>
  <tr>
    <td class="tg-vncu">ADVENT <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf">[6]</a></td>
    <td class="tg-bg24">(soon)</td>
    <td class="tg-8jvv">68,43</td>
  </tr>
  <tr>
    <td class="tg-4dm3">CLAN <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf">[7]</a></td>
    <td class="tg-z8x8">(soon)</td>
    <td class="tg-4dm3">70,30</td>
  </tr>
  <tr>
    <td class="tg-cbs6">DISE <a href="http://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_All_About_Structure_Adapting_Structural_Information_Across_Domains_for_Boosting_CVPR_2019_paper.pdf">[8]</a></td>
    <td class="tg-iml5">(soon)</td>
    <td class="tg-cbs6">73,64</td>
  </tr>
</table>