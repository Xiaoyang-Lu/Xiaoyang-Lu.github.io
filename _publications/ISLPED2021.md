---
title: "CoPIM: A Concurrency-aware PIM Workload Offloading Architecture for Graph Applications"
collection: publications
permalink: /publications/ISLPED2021
venue: "The 2021 IEEE/ACM International Symposium on Low Power Electronics and Design (ISLPED 2021)"
date: 2021-07-26
---

## Abstract

Processing-in-Memory (PIM) is considered a promising solution to improve the performance of graph-computing applications by minimizing the data movement between the host and memory. Which workload to offload and how to offload it to PIM logic determine whether the PIM architecture is well utilized. Offloading too much or too little workload from the host processor to the PIM side could hurt overall performance. On the other hand, the offloading granularity needs to be representative without losing generality. In this paper, we present CoPIM, a novel PIM workload offloading architecture that can dynamically determine which portion of the graph workload can benefit more from PIM-side computation. CoPIM focuses on the loop code blocks of graph applications and evaluates the necessity of offloading based on a concurrent memory access model. We also provide detailed architectural designs to support the offloading. In this way, CoPIM reduces the size of offloading instructions and also improves the overall performance with less energy consumption. The experimental results show that compared with other state-of-the-art PIM workload offloading frameworks, CoPIM achieves a speedup by the geometric mean of 19.5% and 11.4% than PEI and GraphPIM, respectively. On the other hand, CoPIM also reduces the un-core energy consumption by 6.8% and 6.5% on average over PEI and GraphPIM, respectively.

[paper](../files/ISLPED2021/CoPIM_paper.pdf)
