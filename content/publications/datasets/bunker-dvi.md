---
title: Bunker DVI Dataset
type: docs
prev: publications/datasets/
---



![](/images/bunker-dvi-dataset_rig-sample.jpg "Figure 1. Sample frames from different cameras and hardware platform.")



## Introduction 

This dataset was collected for our ongoing research on portable 3D mapping systems based on depth-visual-inertial cameras. Targeting resource and time-constrained mapping operations in adverse conditions (e.g. in the context of search-and-rescue), our sequences include agressive motion, sequences with people moving in the field of view of the sensors as well as sequences with abrupt lighting changes.

Our sensor platform features an extensive set of sensors:

- 3D LiDAR
- Active stereo camera
- Passive stereo camera
- Time-of-flight camera
- Multiple Inertial Measurement Units (IMUs)

With this sensor suite, our dataset allows the comparison of various depth sensing modalities for the task of 3D reconstruction in a challenging and large-scale scenario. The data was captured in a bunker-like location, resembling a typical search-and-rescue operation site. The whole environment is a large, 1600m2 area made of small corridors, rooms of all sizes and shapes and various objects.

The dataset features high-quality ground truth obtained by registering the LiDAR scans in the ground truth map (FARO Focus 3D):

![](/images/bunker-dvi-dataset_whole-map-alt.jpg "Figure 2. Whole map seen by different angles")

![](/images/bunker-dvi-dataset_scan_in_map_gt.jpg "Figure 3. Livox Mid-360 LiDAR scan being registered in the ground truth map")

## Video 
<iframe width="560" height="315" src="https://www.youtube.com/embed/92fUBhA0Cyw" title="Bunker DVI Dataset - Overview" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Links 
- [Dataset website](https://charleshamesse.github.io/bunker-dvi-dataset/)
- [Paper](https://ieeexplore.ieee.org/document/10737432)