---
title: 'Incrementally Building Topological Graphs via Distans Maps'
date: 2018-09-01
permalink: /posts/2018/09/incremental-topo/
tags:
  - map representation
  - distance maps
---

The problem want to solve is to generate the topological map incrementally during the investigation of robot such that the motion planning can benefit from it.

### Incremental Topo

Mapping is an essential task for mobile robots and topological representation often works as a basis for the various applications. In this paper, a novel framework that can build topological maps incrementally is proposed. The algorithm is using a distance map, and in our framework the topological map can grow as we append more sensor data to the map. To demonstrate our algorithm, we show the result of the distance map based method on several popular maps and run the incremental framework with raw sensor data to have a growing topological map, as an example of a robot exploring the environment.

<p align="center">
  <img src="https://jarrome.github.io/files/incrementalTopo.gif?raw=true" alt="Photo" style="width: 800px;"/> 
</p>

* Yuan, Y. & Schwertfeger, S. (2019). Incrementally building topology graphs via distance maps. In 2019 IEEE International Conference on Real-time Computing and Robotics (RCAR). IEEE.

The implementation can be found in [github](https://github.com/STAR-Center/IncrementalTopo).
