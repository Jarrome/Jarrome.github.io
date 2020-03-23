---
title: 'Point Set Registration'
date: 2019-07-01
permalink: /posts/2019/07/psg/
tags:
  - pose estimation
  - regiatration 
---

This is the project during my research visiting at Andread Nuechter's group. The goal is to build efficient feature for very large point cloud matching, e.g., the city data, which is a challenge due to the large size of data and the weak capability of recent descriptor in such a dataset.

To achieve the goal, it consists of two subprojects.

### A new formulating of registration problem
This work provide a non-iterative one-step solution.

Yuan, Y., Borrmann, D., Nüchter, A., & Schwertfeger, S. (2020). Non-iterative One-step Solution for Point Set Registration Problem on Pose Estimation without Correspondence. arXiv preprint arXiv:2003.00457.

### Deep feature by supervising on the one-step solved transformation
By self-supervising, Point Set Local Descriptors is learned.

Yuan, Y., Hou, J., Nüchter, A., & Schwertfeger, S. (2020). Self-supervised Point Set Local Descriptors for Point Cloud Registration. arXiv preprint arXiv: 2003.05199.
