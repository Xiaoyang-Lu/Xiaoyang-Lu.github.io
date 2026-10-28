---
title: "HyPIM: Accelerating Hyperbolic Machine Learning via Processing-In-Memory"
collection: publications
permalink: /publications/CCMCC2026
venue: "2nd IEEE Cross-Disciplinary Conference on Memory-Centric Computing (CCMCC 2026)"
date: 2026-10-28
---

Jinlin Wu, Ferit Ozdaban, Selvanathan Sadhasivam, <b>Xiaoyang Lu</b>, Yunhui Guo, Minxuan Zhou

## Background

Hyperbolic machine learning uses non-Euclidean geometry to represent hierarchical data efficiently, benefiting applications such as graph learning and computer vision. However, existing GPU accelerators are primarily optimized for compute-intensive matrix operations and struggle with the memory-intensive transformations required by hyperbolic models.

In particular, Lorentz-model hyperbolic operations involve frequent data movement, element-wise computations, and reductions. These operations introduce a compute–memory imbalance and substantially underutilize GPU arithmetic resources.


## Design

HyPIM introduces a **GPU–processing-in-memory (PIM) heterogeneous architecture** that accelerates hyperbolic machine learning by matching operations to the hardware best suited for them. Compute-intensive matrix operations remain on the GPU, while memory-bound hyperbolic operations are offloaded to HBM-based PIM units to reduce unnecessary data movement.

HyPIM combines near-bank processing units for vector operations and local reductions with channel-level units for transcendental operations. It further employs a **hyperbolic-friendly data layout** and **in-flight wavefront scheduling** to coordinate heterogeneous operations and improve hardware utilization.

## Key Features

- **Heterogeneous GPU-PIM Execution**: Keeps compute-intensive operations on the GPU and offloads memory-bound hyperbolic operations to PIM.
- **Specialized PIM Units**: Uses bank- or bank-group-level units for vector operations and reductions, with channel-level units for transcendental functions.
- **Data Layout Optimization**: Organizes hyperbolic operands to exploit internal HBM bandwidth and reduce data movement.
- **In-Flight Wavefront Scheduling**: Coordinates different execution stages across PIM units to improve resource utilization.

## Results

Experiments on hyperbolic machine learning workloads demonstrate:

- **3–7× speedup** over an NVIDIA A100 GPU on evaluated HypFormer datasets.
- **Approximately 30% average reduction in total energy consumption** per inference task.

## Conclusion

HyPIM demonstrates how **hardware–software co-design and processing-in-memory** can accelerate hyperbolic machine learning. By combining GPU computation with PIM-based execution of memory-intensive hyperbolic operations, optimized data layouts, and wavefront scheduling, HyPIM reduces data movement and improves the performance and energy efficiency of emerging AI workloads.

[paper](../files/CCMCC2026/CCMCC2026.pdf) | [poster](../files/CCMCC2026/CCMCC2026_poster.pdf)
