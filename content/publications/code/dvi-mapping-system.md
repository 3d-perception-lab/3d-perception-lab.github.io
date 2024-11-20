---
title: Depth-Visual-Inertial Mapping System
linkTitle: Depth-Visual-Inertial Mapping System
type: docs
prev: publications/datasets/
---


## Introduction

We propose the Depth-Visual-Inertial (DVI) mapping system: a robust multi-sensor fusion framework for dense 3D mapping using time-of-flight cameras equipped with RGB and IMU sensors. Inspired by recent developments in real-time LiDAR-based odometry and mapping, our system uses an error-state iterative Kalman filter for state estimation: it processes the inertial sensor's data for state propagation, followed by a state update first using visual-inertial odometry, then depth-based odometry. This sensor fusion scheme makes our system robust to degenerate scenarios (e.g. lack of visual or geometrical features, fast rotations) and to noisy sensor data, like those that can be obtained with off-the-shelf time-of-flight sensors. 

For evaluation, we propose the new [Bunker DVI Dataset](https://charleshamesse.github.io/bunker-dvi-dataset), featuring data from multiple DVI sensors recorded in challenging conditions reflecting search-and-rescue operations.

This video shows the proposed system running on all evaluation sequences of the Bunker DVI Dataset:

<a href="https://www.youtube.com/embed/GzjHYDx21o0" target="_blank"><img src="http://img.youtube.com/vi/GzjHYDx21o0/0.jpg" 
alt="cla" width="640" height="480" border="10" /></a>

This code runs on **Linux**, and is fully integrated with **ROS**. It has been tested with ROS Noetic. In the future, we plan to implement a ROS2 compatible version.

## Links



- Repository: [https://github.com/charleshamesse/dvi-mapping-system/](https://github.com/charleshamesse/dvi-mapping-system/)
- Citations: 
    - **Depth-Visual-Inertial Mapping System for Robust Indoor 3D Reconstruction**<br />
C Hamesse M Vlaminck, H Luong, R Haelterman<br />
*IEEE Robotics and Automation Letters, 2024* 
