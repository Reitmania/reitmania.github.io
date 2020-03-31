---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
<!--
Currently, my research focus is on synthetic data and virtual sensors for lab-based preparation of ML applications for reality. For modeling and data generation I use Blender and own plugins, which I combine with ML algorithms like GANs and AE. During my PhD phase I worked on the prediction of complex time series in aviation, especially by LSTMs. 
I published in several traffic and informatics related journals and participated in international conferences. In addition to my scientific work I am student of Informatics at the University Hagen and game developer in a small game dev studio in Dresden.
-->

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
