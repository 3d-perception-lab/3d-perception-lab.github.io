---
title: Mobile Manipulation for Demining, EOD & IED operations
linkTitle: BELGIAN
type: docs
prev: research/projects/
---

{{% details title="Funding information" %}}

- Source: DFR
- Project code: DAP23/08
- Total cost: 466 k€
- Start date: January 1st, 2024
- End date: December 31st, 2027

{{% /details %}}

**Keywords:** Mines, improvised explosive devices, explosive ordnance, UGV, demining, manipulation

## Context and motivation

The **BELGIAN** project builds on over 2 decades of research activities within the RMA-RAS team on the development of robotics tools for mine clearance. The subject of robotic demining is important for military operations, as still too many lives of soldiers and civilians are lost by these indiscriminate weapons, that continue to be used, as proven recently in the Ukraine conflict, notwithstanding the Ottawa treaty. Aside from the devastating loss in human lives, the use of Improvised Explosive Devices (IEDs), by adversaries also significantly hampers and slows down military operations, as the cleaning process is very slow, tedious and costly.

Within this context, **BELGIAN** must be seen as a direct continuation of the European AIDED project (which in its turn was a follow-on to the European TIRAMISU project). The AIDED project aimsto develop an AI-enabled robotic swarm with advanced EO detection and classification, and automated mission planning capabilities, that can be sent out in advance to detect and classify EOs in the terrain, thereby keeping the human soldiers out of harm’s way. The AIDED system sendsinformation such as position, type and any other information related to the detected IEDs to allow the demining teams to operate according to the data obtained.Still, like in all previous research activities on this domain at RMA-RAS, at the end of the day it is still the human demining expert that has to carry out the fine manipulation on the EO for the disarming operation. This is exactly the capability gap that **BELGIAN** aims to tackle. The aim of the project **BELGIAN** is to capitalize upon the approach ofthe AIDED project by adding semi-autonomous demining robots to the system to carry out the disarming of IEDs directly after their detection.

These **BELGIAN** demining robots should be able to participate in the IED detection phase autonomously and be tele-operable at any time by a member of the demining team to initiate an IED deactivation procedure.In addition, these new demining robots will have to offer innovative and intuitive teleoperation methods using virtual reality. The use of this technology aims to reduce the learning time and improve the manoeuvrability of the demining robots to facilitate the demining manipulations, in particular the control of the manipulator which plays a fundamental role in this procedure.

## Objectives

The global objective of **BELGIAN** is to provide EOD teams with better robotic tools, allowing them to perform remote EO disarming operations. This is achieved by designinga semi-autonomous control system for a multi-robot demining system equipped with robotic arms. The autonomous operation of the multi-robot system will enable rapid IED detection in an unknown and large-scale environment, likely to be dangerous due to the probable presence of IEDs and other explosive systems. The presence of the robotic arm will allow the robots to improve their range of action during their autonomous operation by implementing functionalities such as the ability to open doors with the robotic armor disarm EO, thereby increasing the percentage of EOD operations that can be executed fully remotely and thus without exposing human operators to life-threatening risks

## Project team


| Name | Institution | Role |
|:--|:--|:--|
| Ken HASSELMAN | RMA, RAS Lab | Coordinator |
| Charles HAMESSE | RMA, 3D Perception Lab | Coordinator |
| Mario MALIZIA | RMA, RAS Lab | Research Engineer |


## Output 



### Multi-spectral minefield dataset collection

We have collected a realistic minefield dataset using sensors for 3D perception (localization and mapping) and a multi-spectral camera rig for mine detection. The dataset will be published soon. 

![](/images/belgian_1.jpg "Figure 1. Platform sensors: multi-camera-inertial sensor and LiDAR.")

![](/images/belgian_2.jpg "Figure 2. Arm-mounted sensors: RGB, SWIR and LWIR camera.")

![](/images/belgian_3.jpg "Figure 3. Sample mines (in this case, PFM-1) used in the field.")