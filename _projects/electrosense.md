---
layout: project
title: Electrosense Assisted Robotic Manipulation
date: June 11, 2017
image: pre_grasp.png
---

## Overview

Underwater robotics represent an interesting problem domain that offers its own unique challenges. Computer vision based algorithms that may have been highly effective on land may be rendered ineffective due to low visibility conditions underwater, while on the other end of the spectrum contact based sensing methods may not be ideal due to noise or sensitivities due to vibration. Sonar is a natural, and well-established, alternative to the above two sensing modalities, yet has its own limitation, namely in the case of shorter (cm to meter) length scales. Electrosense, which is a bio-inspired form of sensing based on perturbations of a self-generated AC electric field, is a promising approach to address this blind spot.

For this project, we seek to apply principles of electrosense to assist in various robotic manipulation tasks, such as grasping. The Smith group at UW Seattle [1], has done extensive work on electric field based “pre-touch” grasp planning, which utilizes the electrosense concept to increase the success rate of grasps. We seek to extend this idea to underwater object localization, “pre-touch,” and grasping maneuvers.

## Goals

Electrosense relies on careful interpretation of the electric field perturbations to infer geometric or material properties of the object of interest. Due to the complexity of the data, and moreover the difficulty in deriving fully analytic interpretative models, specific machine learning models could be considered as alternatives. Some related recent work has been published by the Goldberg group, demonstrating grasp planning strategies with deep convolutional neural networks (CNN’s) [2].

It is my overarching goal, for my MSR final project, to compare more traditional (estimation and control based) methods with more contemporary machine learning techniques (such as deep CNN’s) with respect to performance in a manipulation task.

## Progress

This project is still in the early stages, so there are a lot of directions to explore. After delving through the existing literature, I’ve decided to implement a particle filter based approach for target localization. This was inspired by some previous work done in the MacIver lab [3]. While particle filters can be computationally expensive, they can be both a promising first step (being a nonparametric filter, it does not make assumptions about underlying distributions), as well as a benchmark for later work. As a small sub-task, I have the following in mind to accomplish:

    1) Set up a simplified model (2R robot with laser based sensors that return noisy distance estimates), subject to certain assumptions such as fixed world frame and initially unknown target position

    2) Derive the state transition model, measurement model, and noise models

    3) Implement the particle filter algorithm to visualize the particles converging on the true target object location


This is ongoing work, please come back for future updates.


## References

[1] https://sensor.cs.washington.edu/pubs/ML/robotics/an_electric_field_pretouch.pdf
[2] https://arxiv.org/abs/1703.09312
[3] https://pdfs.semanticscholar.org/8916/29180b02bdc7adf967628c98e2cda72a1099.pdf

