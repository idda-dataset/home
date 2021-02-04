---
permalink: /contact/
layout: archive
toc: false
classes: wide
author_profile: false
title: "Contact the team"
excerpt: "Please contact us for any question, information or feedback."
feature_row:
  - image_path: assets/images/avatar1.png
    alt: "Antonio Tavera"
    title: "Antonio Tavera"
    excerpt: "PhD Student in Deep Learning and Computer Vision at **Politecnico di Torino** and **Italdesign**"
    url: "https://taveraantonio.github.io"
    btn_label: "Visit my Page and Contact Me"
    btn_class: "btn--info"
  - image_path: /assets/images/avatar2.png
    alt: "Emanuele Alberti"
    title: "Emanuele Alberti"
    excerpt: "PhD Student in Deep Learning and Computer Vision at **Politecnico di Torino**"
    url: "mailto:emanuele.alberti@polito.it"
    btn_label: "Contact Me"
    btn_class: "btn--info"
feature_row1:
  - image_path: /assets/images/avatar3.png
    alt: "Barbara Caputo"
    title: "Barbara Caputo"
    excerpt: "Full Professor at **Politecnico di Torino**, **IIT** Senior Researcher, Board member of **Ellis Society**"
    url: "mailto:barbara.caputo@polito.it"
    btn_label: "Contact me"
    btn_class: "btn--info"
  - image_path: /assets/images/avatar4.png
    alt: "Carlo Masone"
    title: "Carlo Masone"
    excerpt: "PhD, Roboticist and Autonomous Driving Engineer, ADAS Specialist at **Italdesign**"
    url: "mailto:carlo.masone@italdesign.it"
    btn_label: "Contact Me"
    btn_class: "btn--info"
---


{% include feature_row id="intro" type="center" %}
Please contact us for any question, information or feedback.
{% include feature_row %}
<br>
<br>
# The Laboratory
{% include feature_row id="intro" type="center" %}
## [VANDAL Lab](http://vandal.polito.it)
# The company
{% include feature_row id="intro" type="center" %}
{% for post in site.AboutItaldesign limit: 5 %}
  {% include archive-single.html %}
{% endfor %}