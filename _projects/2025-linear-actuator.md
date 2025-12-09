---
layout: project
title: Linear Actuator Optimization
description: Portfolio creation for ENGRD 2020
technologies: none
image: /assets/images/linear-actuator-sketch.png
---

#### Project Overview and Objective

In ENGRD 2020, students were given the following problem: 

Given a 2D design space of 150cm in length and 50cm tall, a rigid bar of a fixed length (of your choice), three pin supports of which two need to be mounted on the ground and a linear actuator, design a frame/mechanism to lift the maximum possible weight to the highest possible height. Assume all the supports and bar/actuator are rigid.

#### My Approach

In my approach to this problem, I relied mainly on relationships I know between the angle, the height, and the weight lifted. My design starts with a 50 cm rigid bar, in order to maximize height due to the design space being just 50 cm tall. One of the three pins in the design is at the leftmost side of the bar, attached to the ground and the bar. This pin allows for the bars rotation about the z-axis and provides reaction forces and moments in every other sense.

The remaining two pins should be the mounting of the base of the linear actuator to the ground and at the point connecting the top of the linear actuator to the bar. To think about where these pins should be, we should compare the consequences of placing the actuator at different points along the bar. I determined that, because in this case we are only concerned with the maximum height and weight, it is ideal to put the actuator at 50cm, meaning 50 cm to the right of the first pin along the ground and along the bar. With the linear actuator at this point, it will need to extend farther to get the bar up to maximum height compared to if it is placed closer to the center of the bar. However, with the linear actuator placed at the end, the lever arm is maximized in length, allowing for the absolute maximum lift force to equal the desired actuator's force. In this case, the stroke needed will be longer and thus may be more expensive but that will be ignored in this problem in order to maximize height while lifting the maximum weight.

#### Final Design

In the end, I opted to utilize a 50cm bar in order to maximize height along with the RSX linear actuator because it has the ability to exert a force of, up to, 294kN, much greater than the other actuators.

#### Analysis of Beam Deflection

Once the basics of the design have bee decided on I moved on to an analysis of deflection. Recall that originally we assumed that the beam was rigid, this assumption we will no longer hold. This system now represents a pin-pin system with one end being pinned to the ground and the other end being pinned to the linear actuator.

In a pin-pin system, maximum deflection occurs at the midway point between to the two pins that are being considered.

When a mass is added on the bar, the weight acts in the negative j direction. Only the perpendicular components of the weight contribute to the deformation of our bar. This is maximized when theta=0 due to the bar being perpendicular to the weight, meaning the linear actuator is applying a force of 0kN.

[Deflection and Cross Section Analysis]({{"assets/images/statics-portfolio-work.jpg" | relative_url }}){: .inline-image-l style="width: 100%}

Here you can see the work done in analyzing the deformation.

#### Final Design

![Cross Section]({{"assets/images/cross-section-design.png" | relative_url }}){: .inline-image-l style="width: 60%}

We now know how the beam will deform along with the value of I. Using Appendix D from Beer et. al., I would use W150x24 made from rolled steel for my design case as seen below.