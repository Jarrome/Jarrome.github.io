---
title: 'Flipper Planning for Rescue Robots'
date: 2019-04-01
permalink: /posts/2019/04/flipper/
tags:
  - Rescue Robotics
  - Motion Planning
---

This project propose a very inexpensive method on compute the rescue robot morphology (with flipper) in various terrain.

The implementation consists of 1. desgin the morphology can 2. control robot to achieve it. Generally, recent work focus on 2 while use state machine on 1 which is specifically for certain terrain. In this project, we solved the 1 that can deal with different terrain.

consists of initial flipper planning idea (SSRR2019) and flipper planning on 3D terrains.

### Configuration-space Flipper Planning for Rescue Robots

For rescue robots, flipper endows the robot with additional ability to pass through various terrain. Autonomous motion becomes more important. In recent work autonomy is done by either planning with several special states or based on collected data. We are considering if it is possible to find a way to build continues states without collecting old trail data. In this paper, we first model the possible states as a global planning path with parameter configuration of the scene. Then, we follows the path to achieve the autonomous run. We plot the morphology of each path points to show the correctness of the path and implement a simple path following on real robot to demonstrate the performance of our algorithm.

<p align="center">
  <img src="https://jarrome.github.io/files/flipperPlanning.png?raw=true" alt="Photo" style="width: 450px;"/> 
</p>

* Yuan, Y., Wang, L. & Schwertfeger, S. (2019). Configuration-space Flipper Planning for Rescue Robots. In 2019 IEEE International Symposium on Safety, Security, and rescue robotics (SSRR). IEEE.

The implementation can be found in [github](https://github.com/STAR-Center/flipperplanning).

### Configuration-space Flipper Planning on 3D Terrains

Flippers are essential components of tracked robot locomotion systems for unstructured terrain, especially within a rescue scenario. Achieving full and semi-autonomy for such rescue robots is the goal of many research efforts. In this work, we propose an algorithm to plan the morphologies of a small rescue robot with four flippers over 3D ground without any extra sensor, such as pressure sensor. To achieve the goal, we simplify the rescue robot as a skeleton on inflated terrain. Its morphology can be represented by configurations of several parameters. Then we plan the mobile movement on 3D terrain with four individually manipulated flippers. We perform real robot experiments on three different obstacles. The results show that we move the flippers very effectively and are thus able to tackle those terrains very well.

<p align="center">
  <img src="https://jarrome.github.io/files/flipperPlanning3D.png?raw=true" alt="Photo" style="width: 650px;"/> 
</p>

* Yuan, Y., Xu, Q. & Schwertfeger, S. (2019). Configuration-space flipper planning on 3d terrain. ArXiv preprint arXiv:1909.07612.

The source code will be released soon.
