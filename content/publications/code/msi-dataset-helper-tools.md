---
title: Multi-Spectral Inspection Dataset Helper Tools
type: docs
prev: publications/datasets/
math: true
---



## 1. Create the reference map with mine locations

Using the platform sensors only:

```mermaid
graph LR;
    A[LiDAR]-->D(Faster-LIO-ROS2);
    B[IMU]-->D;
    D-->E[Reference global point cloud];
    D-->E2[Timestamped LiDAR poses];
    C[Cameras]-->F(Koide3-Calibration*);
    A-->F;
    C-->A2(AprilTag Detection and Pose Estimation);
    A2-->G(SE3 Transformation);
    F-->G;
    G-->H[Timestamped mine positions in LiDAR frame]
    H-->I(SE3 Transformation*)
    E2-->I
    I-->J[$$^W \bm t_i~ 's$$*]
```

where:
- $^W \mathbf{t}_i \in \mathbb{R}^3$ is the position of the i-th target in the world frame

Nodes marked with a * are not implemented yet. 

## 2. Compute the poses of the platform in the current sequence in the reference map

Using LiDAR-inertial data from the new sequence:

```mermaid
graph LR;
    A[Reference global point cloud from step 1]-->E
    B[LiDAR]-->D
    C[IMU]-->D
    D(LI-SLAM)-->D2[Global map]
    D-->D3[Timestamped LiDAR poses]
    D2-->E
    E(Registration with ICP)--$$^W T_C$$-->H
    D3-->H(SE3 Transformation)
    H-->I[Platform pose in reference map]
```

where:
- $^W T_C$ is the SE3 transformation from current map to world frame (i.e. reference map)


## 3. Project the target positions in the arm cameras

Here shown using the RGB camera as example:
```mermaid
graph LR;
    A[$$^W \bm t_i~ 's$$]-->E
    B[T_mid360_to_avia]-->D2
    C[T_avia_to_rgb]-->D2
    D[T_W_to_mid360]-->D2[T_W_to_rgb]
    D2-->E
    E[SE3 Transformation]-->F
    F["$$^{\textnormal{RGB}} \bm t_i~ 's$$"]-->H
    G[RGB intrinsics $$\bm K$$]-->H("$$\pi(\bm K, ^{\textnormal{RGB}} \bm t_i)$$")
    H-->I["$$^{\textnormal{uv}} \bm t_i$$"]
    
```
where:
- $^{\textnormal{uv}} \bm t_i$ are the coordinates of the i-th target in the image plane of the RGB camera
- $\pi(\bm K, ^{\textnormal{RGB}} \bm t_i)$ is the pinhole camera projection operation
