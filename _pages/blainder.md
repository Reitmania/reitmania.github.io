---
layout: archive
title: "BlAInder"
permalink: /blainder/
author_profile: true
---

> Reitmann, S.; Neumann, L.; Jung, B. BLAINDER—A Blender AI Add-On for Generation of Semantically Labeled Depth-Sensing Data. Sensors 2021, 21, 2144. [https://doi.org/10.3390/s21062144](https://doi.org/10.3390/s21062144) 

> [https://github.com/ln-12/blainder-range-scanner](https://github.com/ln-12/blainder-range-scanner)

One of my overall research goals was that we can use Blender as a synthetic data generator for various machine learning and robotics applications (the project is called **BlAInder**). 

![alt text](../images/blainder2.png "BlAInder Logo")

Due to ML some specific things (labeling & data formats) have to be considered. In order to use Blender for this, different sensors are needed. For the current research in our company these are above all:

- RGB-D cameras (e.g. Kinect)
- LiDAR (surface analysis, see [https://www.blensor.org/](https://www.blensor.org/))
- Sonar (underground analysis, multibeam, singlebeam...)
- Omnidirectional cameras (see [https://github.com/uzh-rpg/rpg_blender_omni_camera](https://github.com/uzh-rpg/rpg_blender_omni_camera))

For all sensors the sensor specs have to be considered as well as the physical limitations. All data has to be labelled, i.e. you get the IDs for each process on Blender and map them to the respective output. This is a unique selling point (e.g. compared to the LiDAR package for ROS). For point clouds, an ID is assigned to each point that is created by a Ray Intersect on an object (LiDAR, sonar), for images (RGB-D, cameras) the information would have to be transferred into the rendered image (as bounding box or pixelwise labels). This can be found, for example, here: [https://arxiv.org/pdf/1709.00849.pdf](https://arxiv.org/pdf/1709.00849.pdf).

Physically it becomes interesting for certain diffuse (black, white) and (semi)transparent materials (especially glass). There are also error models for this. It is also important that the measurements in our projects are carried out in different ways. At [AIRGEMM](https://tu-freiberg.de/airgemm) we partly fly over a water body, partly measure from the robotic boat. There are certain error models and restrictions for both (see e.g. [https://www.neonscience.org/lidar-basics](https://www.neonscience.org/lidar-basics)).

![alt text](../images/suz.png "Mesh representation.")
![alt text](../images/suz2.png "LiDAR point cloud.")
![alt text](../images/suz3.png "LiDAR labeled point cloud.")

The quality of the scene depends on the sensor. For point clouds and depth images, meshes made of critical materials, such as glass, are mostly sufficient. For real image analysis the rendering would have to be of higher quality, but that would not be part of the MA. If the images were added, colored primitives against white background would be sufficient or something like that. 

The programming goal is a plugin for Blender. The similar project Blensor added all the Ray methods in C++ via patch and then implemented a Python plugin for UI and programming. Something similar is in my mind. This is performant and accessible. Blensor is outdated and has only limited functionality, but it is a good basis. 

# Data Export

The simulated data must be saved for later use. In addition to the point data itself, information about the objects through which the respective point was created is also necessary. Also the color of the original object at the point of intersection with the emitted beam as well as the distance to the sensor should be included for later visualization. Various file formats are provided for this purpose.

A common format for machine learning applications is the "Hierarchical Data Format" (short: HDF). The advantages are the management of heterogeneous data, the self-describing structure of the data format including additional metadata, the platform independence as well as the support and extension by numerous software projects. For example, "h5py" is a library for using the file format in Python. Furthermore the support of the LAS format is planned. This format was developed by the "American Society for Photogrammetry and Remote Sensing", is designed for the storage of three-dimensional tuples and is a common format for storing lidar point clouds. Among other things, it can be used to create three-dimensional visualizations with the help of the program "Potree". A connection to Python is provided by the library "laspy". The third desired format for export is a simple text format. In this format the tuples of coordinates and additional information can be stored line by line.
