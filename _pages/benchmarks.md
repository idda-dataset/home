---
permalink: /benchmarks/
layout: splash
toc: false
author_profile: false
title: "Benchmarks"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/benchmark.jpg
---


% for post in site.posts limit: 5 %}
  {% include archive-single.html %}
{% endfor %}

{% include feature_row id="intro" type="center" %}