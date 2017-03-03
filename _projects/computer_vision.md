---
layout: project
title: Computer Vision Projects
date: September 24, 2015
image: RANSAC_hw3_larger.png
---

## Overview

Here are three projects I implemented for the Computer Vision and Computational Photography course I took Fall 2015 at the University of Pennsylvania.

### Disclaimer
I did not provide the MATLAB scripts for these projects publicly (github, etc.)
since these projects are still used as homework assignments for the course.

### Canny Edge Detection

![canny_image](https://github.com/ShiL1617/ShiL1617.github.io/blob/master/public/images/mycanny.jpg)

This was my custom implementation of the Canny edge detection algorithm.

We had followed the approach outlined in the original paper, but were
given freedom on how to implement the various steps within the algorithm.
I had taken different approaches to image filtering and edge linking
hysteresis, which greatly assisted in detection of low-frequency edges.


### Image Warping

![imwarp_image](https://github.com/ShiL1617/ShiL1617.github.io/blob/master/public/images/ctr_pts_TPS.png)

For this project, I implemented two approaches for image warping
(transforming one image into another): Delaunay triangulation/barycentric
coordinates, and thin plate spline (TPS) methods.

Since this project was completed around Halloween, I decided it'd be
fun, and appropriate, to transform a human face (mine) to a wolf face. While
there were promising results with the triangulation methods, TPS introduced
some issues with correspondence points (equivalent feature points on each face).This was attributed to topological distortions due to drastically different
feature arrangements on a global scale.


### Image Stitching

![RANSAC_image](https://github.com/ShiL1617/ShiL1617.github.io/blob/master/public/images/RANSAC_hw3_larger.png)

Through this project, we created our own image panoramas, relying on techniques
in feature detection/matching, homographies, and RANSAC algorithms.
