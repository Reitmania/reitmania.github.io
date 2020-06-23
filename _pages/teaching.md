---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

## List of supervised theses:
* Generation of 3D training data for AI applications by simulation of ranging methods in virtual environments (Master Thesis, Freiberg University of Mining & Technology)
* Deep Learning for Online Defect Detection in a Ceramic Tape Casting Process (Bachelor Thesis, Freiberg University of Mining & Technology, Fraunhofer)

{% include base_path %}

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}
