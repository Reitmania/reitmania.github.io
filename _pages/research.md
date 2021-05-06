---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

> Currently, my research focus is on synthetic data and virtual sensors for lab-based preparation of ML applications for reality. For modeling and data generation I use Blender and own plugins, which I combine with ML algorithms like GANs and AE. I mainly code in Python and C++. For ML applications I use TensorFlow, sklearn, pytorch and YOLO. I regularly work with the game engines UE4 and Godot and use the software Blender to design and simulate virtual worlds.

## Machine learning in time series prediction

 In my doctoral thesis I dealt with the application of neural networks (MLP, RNN/LSTM, hybrids) in time series prediction in air traffic. Besides multidimensional modeling, I have been able to extract knowledge from neural networks by using genetic algorithms. 
 
 You can find my PhD thesis [here](https://nbn-resolving.org/urn:nbn:de:bsz:14-qucosa2-729299).
 
<center>
<img src="../images/research/vATM1.png" alt="Mesh" width="400"/>
<img src="../images/research/vATM2.png" alt="Point Cloud" width="400"/>
</center>

## Machine learning in computer vision 

In my habilitation thesis I apply machine learning methods on complex geophysical data sets. Scientific and technical goals concern e.g. the development of AI-based prediction methods for the detection of disturbances and boundary layers. These predictions will form the basis for significantly more efficient simulations, e.g. for solving of inverse problems in the area of electromagnetic geophysics. Further work addresses e.g. automated data processing workflows to establish model-driven machine learning pipelines using heterogenous geological data repositories.

You can find more information about our project AIRGEMM (*AI and Robotics for GeoEnvironmental Modeling and Monitoring*) [here](https://tu-freiberg.de/airgemm).

<center>
    <img src="../images/suz.png" alt="Mesh" width="250"/>
    <img src="../images/suz2.png" alt="Point cloud" width="250"/>
    <img src="../images/suz3.png" alt="Labeled point cloud" width="250"/>
</center>

## AI in virtual worlds 

In order to train virtual agents in artificial worlds, I develop concepts to bring them into suitable environments and to transfer the AI trained there to the outside. For this purpose, the game engine **Godot** is used. Within my research I develop frameworks for Godot to create an interference engine for ANN. Furthermore, agents will be trained by reinforcement learning. I create the virtual environments with Blender and incorporate models of my colleagues, which provide a very realistic image with photogrammetry.

<center>
<img src="../images/LA2020.png" alt="LA2020" width="400"/>
</center>

## VR/AR

For a better understanding of the measurements of our robotic boat and their visualization, we are in the development of an AR application. Thereby, measured point clouds are to be displayed correctly from the edge of the bank at the target water body and registered into the environment. On the one hand, this involves a live view of a measurement run, and on the other hand, the display of an already measured set of points in their entirety. 

A Microsoft HoloLens 2 (HL2) is used as AR hardware, whereby this is to be used as a stand-alone solution, i.e. without an external computing unit. This concept allows mobile applications at the waters, but limits the display scope of the point clouds (according to empirical values, a maximum of 300,000 points). The application is implemented as a Unity application and uses the pcx-Point Cloud Importer [https://github.com/keijiro/Pcx](https://github.com/keijiro/Pcx) to display the point clouds. 



<!--

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>



{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
-->
