---
title: MIXRS
type: docs
prev: research/projects/
---

## Military Intelligent eXtended Reality Systems

{{% details title="Funding information" %}}

- Source: Royal Higher Institute for Defence (RHID)
- Project code: DAP18/04
- Total cost: 0.8 M€
- Start date: January 1st, 2019
- End date: October 31st, 2023

{{% /details %}}

**Keywords:** augmented reality, virtual reality, 3D perception


## Context and motivation

Asymmetric warfare situations and the continuous risk of terrorist attacks place Belgian Defence soldiers in dangerous situations where they have to correctly assess very complex situations in a minimum of time. Advanced sensors like visual and thermal cameras and sensing vectors like RPAS are being deployed to remedy this problem, but these also add to the information overload that soldiers need to process. In its original form, this research study proposed to develop an extended reality support system that assists individual soldiers in collecting, processing and analysing data without taking their eyes and attention from their environment and without causing cognitive overload.

Due to a spark of interest in Virtual Reality (VR) technology from the different Components of the Belgian Defense since the start of this study, the addition of a VR component to this study proposal is requested. In fact, VR opens the way for a new class of training and simulations with multiple advantages over traditional training such as increased availability, realism, repeatability and objectivity. Partnering up with an industrial partner (OneBonsai) in a Triple Helix framework, high-TRL VR systems will be put at the disposal of Belgian Defence clients to answer a recurring and growing demand.

The proposed study will research cross-domain scientific innovations in the fields of computer vision, robotics, human-system integration, machine learning to develop an augmented and virtual reality support system that will support the soldier in each phase of the sense-plan-act decision chain. As a result of this study, Belgian Defence will have at its disposal a proof-of-concept augmented reality system consisting of COTS/MOTS hardware and a custom software augmented reality toolbox, together with multiple Virtual Reality training platforms tailored to the needs of Belgian Defence clients. 

## Objectives

This study proposes cross-domain and cross-cutting research, spanning the research fields of computer vision, mathematics, robotics, data management and human system integration and proposing a differentiated mix of highly scientifically innovative contributions (real-time calibration, high-accuracy localization of team-mates and potentially occluded objects, machine-learning on low-power devices) and higher-Technology Readiness Level innovations which can have a direct impact on the soldier’s performance on the terrain (2D Augmented Reality applications like camera sharing, approximate localization of teammates). 
Human factors are a crucial aspect for the success of the proposed study, as the adoption of the system on the field by the soldiers stands of falls with thorough human-system integration. Therefore, we will follow an iterative development process by having regular interim design review meetings with the clients, developing, and integrating the necessary hardware and software toolboxes as a prototype system that will be validated by the end users and further optimized during the experiments. Finally, the optimized prototype model will be tested and validated in a demonstration scenario together with the Defence units. Collection of extensive experimental data sets during the trial campaigns can be shared with relevant stakeholders for further benchmarking purposes. At various periods during the study there will be opportunities to publish relevant research results.


## Project team

| Name | Institution | Role |
|:--|:--|:--|
| Rob HAELTERMAN | RMA, Hyper RU & 3D Perception Lab | Coordinator |
| Geert DE CUBBER | RMA, RAS Lab | Coordinator |
| Timothée FREVILLE | RMA, 3D Perception Lab | Research Engineer |
| Charles HAMESSE | RMA, 3D Perception Lab | Research Engineer |


## Output

### 3D mapping systems 


We have implemented 3D mapping methods using different sensors and studied their performance in difficult, dynamic conditions.

![](/images/mixrs-rigs.jpg "Figure 1: Various prototype sensor rigs for 3D mapping developed in the context of MIXRS.")

Various papers were published based on our findings:

- **From Depth Sensing to Deep Depth Estimation for 3D Reconstruction: Open Challenges**<br />
C Hamesse, H Luong, R Haelterman<br />
*Proceedings of the 13rd International Conference on Image Processing and Vision Engineering (IMPROVE), 2024*


- **Practical Deep Feature-Based Visual-Inertial Odometry**<br />
C Hamesse, M Vlaminck, H Luong, R Haelterman<br />
*13th International Conference on Pattern Recognition Applications and Methods (ICPRAM), 2024*


- **Development of Ultra-Portable 3D Mapping Systems for Emergency Services**<br />
C Hamesse, T Fréville, J Saarinen, M Vlaminck, H Luong, R Haelterman<br />
*IEEE ICRA Workshop on Field Robotics, 2024*


### Shoothouse

![](/images/mixrs_shoothouse-2.png "Figure 2: Illustration of the VR Shoothouse developed in the context of MIXRS.")

The Belgian Special Forces often need to intervene in unknown environments. Sometimes this requires entering buildings or ships for a first time, which are only known from plans. This procedure brings constraints in terms of safety and needs to be performed and repeated ahead. The aim of this research is to develop a VR simulation for the Belgian Defense to train soldiers to perform multiple scenarios on a 3D reconstruction of a building or ship.

The Special Forces are currently repeating different scenarios in a physical shoothouse for their training. In this environment they can perform hostage and inspection situations. The drawback of such a traditional shoothouse is that they cannot change their layout easily, which makes the trainees too comfortable and used to the same area.

The aim of this project is to create a Virtual Reality Shoothouse. Based on a 2D floorplan or a 3D plan of a building or a boat, an algorithm that features Artificial Intelligence and Image processing will recreate a 3D simulation of it. In this environment, the trainees will perform their approach using VR headsets while being watched and supervised by an overseer who can see the decision making of his troops. With this project we ensure a more versatile environment for inspection procedures where Special Forces can perform any intervention in virtually millions of different layouts without getting too comfortable with it.

![](/images/mixrs_shoothouse-1.png "Figure 3: Illustration of the floor plan to VR environment creation tool.")

- **Object Detection in Floor Plans for Automated VR Environment Generation**<br />
T Fréville, C Hamesse, B Pairet, and R Haelterman<br />
Proceedings of the 18th International Joint Conference on Computer Vision, Imaging and Computer Graphics Theory and Applications (VISIGRAPP), 2023

- **From Floor Plans to Virtual Reality**<br />
T Fréville, C Hamesse, B Pairet, R Lahouli, and R Haelterman<br />
IEEE International Conference on Artificial Intelligence and Virtual Reality (AIVR), 2021


### RTRMA 




We have partnered up with the Belgian Navy in the development of an innovation project around the use of smart glasses for Real-Time Remote Maintenance Assistance (RTRMA). The proposed system was made of two components are proposed: 
- The system for the technician, or maintenance operator, featuring Iristick Z1 smart glasses and a dedicated smartphone app
- The system for the expert, with a dedicated web app. Thanks to the central camera of the smart glasses, the technician streams a video of what they see directly in real-time. The expert can then assist, capture images, annotate and send various documentation back to the onboard technician.

<iframe width="750" height="422" src="https://www.youtube.com/embed/_GyzbKarabI" title="Real-Time Remote Maintenance Assistance (RTRMA)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>