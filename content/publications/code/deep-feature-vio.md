---
title: Deep Feature-Based Visual-Inertial Odometry
linktitle: Deep Feature-Based VIO
type: docs
prev: publications/datasets/
---


## Introduction

We present a hybrid visual-inertial odometry system that relies on a state-of-the-art deep feature matching front-end and a traditional visual-inertial optimization back-end. More precisely, we develop a fully-fledged feature tracker based on the recent SuperPoint and LightGlue neural networks, that can be plugged directly to the estimation back-end of VINS-Mono. By default, this feature tracker returns extremely abundant matches. To bound the computational complexity of the back-end optimization, limiting the number of used matches is desirable. Therefore, we explore various methods to filter the matches while maintaining a high visual-inertial odometry performance. We run extensive tests on the EuRoC machine hall and Vicon room datasets, showing that our system achieves state-of-the-art odometry performance according to relative pose errors.

## Links



- Repository: [https://github.com/charleshamesse/LightGlue-VINS-Mono](https://github.com/charleshamesse/LightGlue-VINS-Mono)
- Citations: 
    - **Practical Deep Feature-Based Visual-Inertial Odometry**<br />
C Hamesse, M Vlaminck, H Luong, R Haelterman<br />
*13th International Conference on Pattern Recognition Applications and Methods (ICPRAM), 2024*

