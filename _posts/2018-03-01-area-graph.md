---
title: 'Area Graph'
date: 2018-03-01
permalink: /posts/2018/03/area-graph/
tags:
  - map representation
  - area shape
---

This project consists of area graph (ICAR 2019), passage graph and hierarchical area graph (My bachelor thesis).

### Area Graph
Representing a scanned map of the real environ- ment as a topological structure is an important research topic in robotics. Since topological representations of maps save a huge amount of map storage space and online computing time, they are widely used in fields such as path planning, map matching, and semantic mapping.
We use a topological map representation, the Area Graph, in which the vertices represent areas and edges represent passages. The Area Graph is developed from a pruned Voronoi Graph, the Topology Graph. We also employ a simple room detection algorithm to compensate the fact that the Voronoi Graph gets unstable in open areas. We claim that our area segmentation method is superior to state-of-the-art approaches in complex indoor environments and support this claim with a number of experiments.

<p align="center">
  <img src="https://jarrome.github.io/files/areaGraph.png?raw=true" alt="Photo" style="width: 650px;"/> 
</p>

* Hou, j., Yuan, Y. & Schwertfeger, S. (2019). Area graph: Generation of topological maps using the voronoi diagram. In 2019 IEEE International Conference on Advanced Robotics (ICAR). IEEE.

The implementation can be found in [github](https://github.com/STAR-Center/areaGraph).
